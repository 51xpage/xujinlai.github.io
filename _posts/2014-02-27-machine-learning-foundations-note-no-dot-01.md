---
layout: post
title: "Machine Learning Foundations note No.01"
description: "ѧϰcoursera�������ѧϰ��ʯ�γ̵ıʼ�"
modified: 2014-02-27 06:14:13 +0800
category:
tags: [ML, note]
image:
  feature: http://seeksky.qiniudn.com/19.jpg-clip.jpg
  credit:
  creditlink:
comments: true
share: true
---

### ǰ��
���ʱ�俴��coursera����`����ѧϰ��ʯ`���ſγ̵��������,����������һЩ��¼

<!--more-->

### ��һ��: The Learning Problem

����ѧϰ��һ���ǳ�ǿ��Ĺ���,���������������,���ǻ�Ҫ���ʼ�������:

 + **When** Can Machines Learn? (illustrative + technical)
 + **Why** Can Machines Learn? (theoretical + illustrative)
 + **How** Can Machines Learn? (technical + practical)
 + How Can Machines Learn **Better**? (practical + theoretical)

����γ̽�Χ�ƽ����⼸������չ��

<iframe src="https://docs.google.com/file/d/0B9qw8YyWZEzKbVZpRzBveEZicDg/preview" width="640" height="480"></iframe>

��һ����Ҫ�����˻���ѧϰ����γ̽�Ҫ���ܵ������Լ��Ի���ѧϰ�����˼򵥵Ľ�ģ.\\
������Ҫ��������һ��ͼ:\\
![]( {{ site.qiniu }}\MLF\defML.png)

���ͼ��Ҫ���������漸������:

 + input: $$x \in X$$ (customer application)
 + output: $$y \in Y$$ (good/bad after approving credit card)
 + **unknown pattern to be learned = target function**:\\
   * $$f : X \to Y$$ (ideal credit approval formula)
 + **data = training examples**: $$D = {f(x_1; y_1); (x_2; y_2); \cdots ; (x_N; y_N)}$$ (historical records in bank)
 + **hypothesis = skill** with hopefully **good performance**:
   * $$g : X \to Y$$ (��learned�� formula to be used)

 + target f unknown
 + hypothesis g hopefully $$\approx$$ f, but possibly **different** from f, (perfection ��impossible�� when f unknown)
 + assume $$g \to H = {h_k}$$
 + hypothesis set H:
   * can contain **good or bad hypotheses**
   * up to A to pick the ��best�� one as g

���ͼ�ܵ���˵���������˻���ѧϰ��ģ��,�����ݵ�**g**����,Ҳ���Ƕ���**f**�Ĳ���.�м��ѧϰģ�;���**A**��**H**.

 + ����ܽ���������: `machine learning`: use **data** to compute **hypothesis _g_** that approximates **target _f_**
