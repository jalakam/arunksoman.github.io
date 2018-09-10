---
layout: post
title: "Maths Trick: Find out Square of a Number"
date: 2018-09-19 23:07:39 -0700
category: Vedic_Mathematics
img: /static/img/maths2.jpeg
mathml: true
color: deep-purple
theme_color: "#673ab7"
tags: 
- Mathematics
- Tricks
---

It is easy to calculate **square of a number** without using calculator. It is not easy to find out square of any number using method described here. The numbers near to powers of 10 can be calculated using this method easily and fast. Here the powers of 10 is taken as reference number to calculate square of a number. To calculate square of number following steps should be followed;

1. Find difference between number to be squared and nearest power of 10. Note down this difference.
2. Find out difference between number to be squared and difference found on first step. Note down this number
3. Find the square of difference got on step 1. Note down this number.
4. Concatenate numbers found on step 2 and step 3.

For example find out square of 94,
1. The nearest power of 10 to 94 is 100. So our reference number is 100 here. Difference between 94 and 100 is 6.
2. 94-6=88
3. Square of 6 is {% include mathml.html math="\[6^{2}=36\]" %}.
4. Concatenating results got on step 2 and step 3 gives {% include mathml.html math="\[94^{2}=8836\]" %}

For another example, find out square of 99
1. The nearest power of 10 to 99 is 100. So our reference number is again 100. Difference between 99 and 100 is 1.
2. 99-1=98
3. Square of 1 is 1
4. But concatenating results on step 2 and step 3 gives {% include mathml.html math="\[\color{red}{981\times}\]" %}. But it is incorrect. You can find out it is incorrect only with inspection since from square of 30 we met 900. {% include mathml.html math="\[99^{2}\]" %} will be a 4 digit number. Since {% include mathml.html math="\[100^{2}\]" %} is 10000 which is a five digit number. (These kind of calculations can be done only using some inspections and previous knowledges and from practice.) The correct result is a 4 digit number. So make the results so add a zero before 1 on step 3. That is correct result is {% include mathml.html math="\[\color{green}{9801 \checkmark}\]" %}.

As an last example consider {% include mathml.html math="\[102^{2}\]" %}. Here only difference is 102 exceeds nearest reference number(i.e., 100) by 2. So the steps will changes like this;
1. Difference between 102 and 100 is 2
2. 102+2=104
3. Square of two is 04(zero is added as prefix for making result a 5 digit number)
4. Concatenating results will give {% include mathml.html math="\[102^{2} = 10404\]" %}
