<script type="text/javascript" src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=default"></script>
# Presentation of Fan Yimin
## Infomation
This is the presentation section prepared by **Fan Yimin(PB17000047)** for the **Signals and Systems** course in USTC,2019 spring.
***
## Topic
### Homework
>1.21 (d)(e)(f)  
1.22 (d)(g)(h)
***
## Basic forms of that kind of problems
### 1.Combination of different signals,especially the combination with **special signals**(*impulse signal,unit step signal,etc*).

>1.21 (f)
### 2.Use of various signal operations,especially **shifting,scaling and reversal**.
>1.21 (d) 1.22(d)(g)
### 3.Transform on the **time domain**.
> 1.22 (h)
### 4.Comprehensive problems.
> 1.21(e)  
 (combination of signal reversal and properties of $u(t)$)
 ***
## Basic ways of solving the problem

### 1. Make use of the properties of the special signals  
*eg:* 
$$ x(t)\delta(t-t_{0})=x(t_{0})\delta (t-t_{0})$$  
$$\quad for\quad t>t_{0}:\qquad x(t)u(t-t_{0})=x(t)$$  
$$for\quad t<t_{0}:\qquad x(t)u(t-t_{0})=0$$
### 2. Make use of the signal operations
*eg:*  
$$\quad shifting,reversal,scaling $$
    
$$add/minus/times \quad a\quad signal/constant$$  
$$... $$
### 3. Transform on the time domain
*eg:*
$$ t_{0}\rightarrow x(t_{0})$$

To find the figure of 
$$x(f(t))$$

Consider 
$$f(t^{'})\rightarrow x(t_{0})\quad  and\quad f(t^{'})=t_{0}$$

So we can find that
$$t^{'}=f^{-1}(t_{0})$$
So we can show that given values at some points of a signal
$$x(t):
{(t_{1},x(t_{1})),}
{(t_{2},x(t_{2})),
{(t_{3},x(t_{3}))...((t_{n}),x(t_{n}))}
}
$$
Signal $$x(f(t))$$ will have these points:
$${(f^{-1}(t_{1}),x(t_{1})),}
{(f^{-1}(t_{2}),x(t_{2})),
{(f^{-1}(t_{3}),x(t_{3}))...((f^{-1}(t_{n}),x(t_{n}))}
}
$$
This method is useful only when:$f(t)$
is invertible $x(t)$ is continuous time signal
However,we can still make use of it even when this condition doen not hold true(eg:1.22(h)).
***
## 1.21
>A continuous time signal x(t)is shown in Figure P1.21.Sketch and label carefully each of the following signals  

![](http://home.ustc.edu.cn/~fym0503/ss/xt.png)
###  $(d)\quad x(4-t/2)$
1.Using scaling,time reversal,shifting.  
Basically,these three oprations will work as follows:  
>shifting  

![](http://home.ustc.edu.cn/~fym0503/ss/com44.png)  

>time reversal

![](http://home.ustc.edu.cn/~fym0503/ss/com22.png)  

>scaling

![](http://home.ustc.edu.cn/~fym0503/ss/com33.png)  

I will not do the 6 orders of these oprations one by one,which is tedious and have a lot in common with the *additional problems*,so I will just show you two of them.
>the yellow signal is the original signal  
the blue signal is the second signal  
the green signal is the third signal  
the red signal is the final signal  

a.*shifting-->reversal-->scaling*  

![](http://home.ustc.edu.cn/~fym0503/ss/com44.png)

![](http://home.ustc.edu.cn/~fym0503/ss/com55.png)

![](http://home.ustc.edu.cn/~fym0503/ss/com66.png)  

b.
*reversal-->scaling-->shifting*  

![](http://home.ustc.edu.cn/~fym0503/ss/com22.png)  

![](http://home.ustc.edu.cn/~fym0503/ss/com88.png)  

![](http://home.ustc.edu.cn/~fym0503/ss/com77.png)  

***Personally,I think it is especially important to notice the differences between different orders of operations.***  
eg:
$$x(at+b)\quad a>0$$  
If we do the shifting $+b$ first,then we just scale the shifted signal with $*a$,However,if we do the scaling $*a$ first,we must shift the scaled signal with $+(b/a)$,and this point confused me when I first learned it.  
And the final result:  
![](http://home.ustc.edu.cn/~fym0503/ss/comparison.png)  

2.Using transformation on the time domain:
From the method I introduced before,in this problem： 
$$f(t)=4-t/2$$
And of course:
$$f^{-1}(t)=8-2t$$
Some points of x(t) is listed below(*Here I just choose some points that are easy to compute and are the turning points*):
| $t$ | $f^{-1}(t)$| $x(t)$ | 
| - | :-: | -: | 
| -2 | 12| 0 | 
| -2 |12 |-1 | 
| -1 | 10 | 0 |
|-1|10|1|
|0|8|1|
|0|8|2|
|1|6|1|
|1|6|2|
|2|4|0|

Draw the scatter:  

![](http://home.ustc.edu.cn/~fym0503/ss/sss.png)  

![](http://home.ustc.edu.cn/~fym0503/ss/ss1.png)



>Note that **mathematically**,this method is **not strict** and will not be helpful in many situations,however,when we do problems in our homework,it is a efficent way to reduce mistakes and help you examine the result of your signal operations.
***
###  $(e)\quad [x(t)+x(-t)]u(t)$
Basically,this problem can be solved by using the signal operation(*reversal,add a signal*)and the properties of $u(t)$.  
(a)find $x(-t)$by using time reversal  

![](http://home.ustc.edu.cn/~fym0503/ss/com22.png)  

(b)adding $x(t)$ and $x(-t)$  

 ![](http://home.ustc.edu.cn/~fym0503/ss/pp.png)  

*It is obvoius that $x(t)+x(-t)$ is an even signal for it is equal to the double of the even part of x(t)*  

(c)times the signal $u(t)$,in fact it is cutting off the left part of $x(t)+x(-t)$  

![](http://home.ustc.edu.cn/~fym0503/ss/xx.png)  

***
### $(f)\quad x(t)(\delta(t+3/2)-\delta(t-3/2))$  

As we know :
>$$x(t)\delta(t-t_{0})=x(t_{0})\delta(t-t_{0})$$  
  

So:  
$$x(t)(\delta(t+3/2)-\delta(t-3/2))\\=x(-3/2)\delta(t+3/2)-x(3/2)\delta(t-3/2))\\=0\quad  when  \quad t>3/2\\=-x(3/2)\delta(0)\quad  when \quad t=3/2\\=0\quad when\quad t>-3/2\quad and\quad t<3/2\\=x(-3/2)\delta(0)\quad when\quad t=-3/2\\=0\quad when\quad t<-3/2 $$
So the figure is shown as below  

![](http://home.ustc.edu.cn/~fym0503/ss/ff.JPG)  

***
## 1.22
>A discrete-time signal is shown in Figure P1.22.Sketch and lable carefully each of the following signals.  

![](http://home.ustc.edu.cn/~fym0503/ss/new0.jpg)  

### $(d)\quad x[3n+1]$  
In fact,by using the same signal operations,such as ***scaling,shifting and reversal***,we can process this discrete time signal as well.However,there may be some problems when you do these kind of this operations,because $x[3n+1]$ will only take values at integer time,which may cause a little confusion.And if we use the transformation,there will also be some problems because $f^{-1}(n)$ may not be integer. So I will show you another way of doing it.  
Firstly,find the time domain when $x[n]$ is non-zero:
$$-4<n<3$$   
Secondly,replace $n$ with $f(n)$ and solve that inequation: 
$$-4<3n+1<3$$  
$$-5/3<n<2/3$$
$$n=0,-1$$
Thirdly,note that the soultion to that inequality is actuall is the non-zero time domain of $x[3n+1]$ ,so just compute the points:  
$$n=0,x[3n+1]=x[1]=1$$  
$$n=-1,x[3n+1]=x[-2]=0.5$$  
the figure is shown as below:  

![](http://home.ustc.edu.cn/~fym0503/ss/hs.JPG)  

from that problem we can conclude a quick wan to draw the figure of $x[an+b]$ in general.  
***
### $(g) \frac 12 x[n]+ \frac 12(-1)^{n}x[n]$  

We know that the figure depends on the value of n, for $(-1)^{n}$ is one when $n$ is even and is minus one when $n$ is odd.  
$$\quad \frac 12 x[n]+ \frac 12(-1)^{n}x[n]\\\quad \quad=\frac 12 x[n]+ \frac 12x[n]=x[n]\quad n\quad is\quad even\\=\frac 12 x[n]-\frac 12x[n]=0\quad n\quad is\quad odd$$ 
So this signal takes $x[n]$ when $n$ is even and takes zero when $n$ is odd.  
The figure is shown as below:  

![](http://home.ustc.edu.cn/~fym0503/ss/new1.JPG)  

***
### $(h) x[(n-1)^{2}]$  
Basically,we will use the same method as (d).And this method is especially useful for (h) because $(n-1)^{2}$ is not linear function so we can not use time shifting,reversal and scaling,and $(n-1)^{2}$ is not invertible,so we can not use the transformation on the time domain.  
Firstly,find the time domain when $x[n]$ is non-zero:
$$-4<n<3$$   
Secondly,replace $n$ with $f(n)$ and solve that inequation:  
$$-4<(n-1)^{2}<3$$  
$$-\sqrt 3<n-1< \sqrt 3$$
$$-\sqrt 3+1<n< \sqrt 3+1$$
$$n=0,1,2$$  
Thirdly,note that the soultion to that inequality is actuall is the non-zero time domain of $x[(n-1)^{2}]$ ,so just compute the points:  
$$n=0,x_{1}[n]=x[(n-1)^{2}]=x[1]=1$$  
$$n=1,x_{1}[n]=x[(n-1)^{2}]=x[0]=1$$ 
$$n=2,x_{1}[n]=x[(n-1)^{2}]=x[1]=1$$ 
the figure is shown as below:  

![](http://home.ustc.edu.cn/~fym0503/ss/new2.JPG)  

I have not thought of another way of solving that problem,if you have one,please tell me.
***
***Sincere thanks for  Prof. Li and Prof.Chen for their teaching and devotion!***





















