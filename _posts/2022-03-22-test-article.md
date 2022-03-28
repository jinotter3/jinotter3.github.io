---
layout: post
title: Test article
subtitle: testing code 
categories: markdown
tags: [test, flutter, dart]
---

## This is test article

* dart test code
{% highlight dart %}
void main();
{% endhighlight %}

~~~dart
import 'package:flutter/material.dart';

class MyPageScreen extends StatelessWidget {
  static const routeName = '/my-page';
  const MyPageScreen({Key? key}) : super(key: key);

  @override
  Widget build(BuildContext context) {
    return Center(
      child: Text('MyPage'),
    );
  }
}

~~~

* matrix multiplication
{% highlight python %}
def g11(matrix1, matrix2):
    mul = []
    for i in range(len(matrix1)):
        row = []
        for j in range(len(matrix2[0])):
            sum = 0
            for k in range(len(matrix2)):
                sum += matrix1[i][k] * matrix2[k][j]
            row.append(sum)
        mul.append(row)
    print(mul)
{% endhighlight %}

~~~python
def g11(matrix1, matrix2):
    mul = []
    for i in range(len(matrix1)):
        row = []
        for j in range(len(matrix2[0])):
            sum = 0
            for k in range(len(matrix2)):
                sum += matrix1[i][k] * matrix2[k][j]
            row.append(sum)
        mul.append(row)
    print(mul)

~~~

