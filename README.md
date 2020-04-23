






Lab1# 09/01/2020



In [1]:



print("Hello")
print('Hello');






Hello
Hello




In [2]:



a=10
b=2.20
c=a*b*a
print(c)






220.0




In [10]:



print(type(b))
print(type(c))
print(type(a))
print(type("Hi"))
print(type('H'))






<class 'float'>
<class 'float'>
<class 'int'>
<class 'str'>
<class 'str'>




In [13]:



print(type(4-2*2+2/4))
print(type(6*5+4%2-3))
print(type(4*2+8/4))
print(type(3+6*5.2/2))






<class 'float'>
<class 'int'>
<class 'float'>
<class 'float'>




In [32]:



x=10.5
y=2.5
print(x/y)
print(x//y)
print(x*y)
print(x**y)
print(type(1j))






4.2
4.0
26.25
357.2508309997333
<class 'complex'>




In [38]:



x=range(6)
print(x)
type(x)






range(0, 6)



Out[38]:

range



In [61]:



a="Bhanu "
b="Prakash Jha"
c=a+b
print(c)
print(c[-1])    #took the last index element
print(c[0:5])
print(c[2:])
print(c[:2])
print(c[0:-6])






Bhanu Prakash Jha
a
Bhanu
anu Prakash Jha
Bh
Bhanu Praka




In [91]:



import random
print(random.randrange(1,7))






6







lab2#15-jan-2020



In [3]:



a="MATHS"
if('M' in a):
    print("M is present in ",a)
else:
    print("M is not present in ",a)






M is present in  MATHS




In [19]:



a=eval(input("enter a-"))
b=eval(input("enter b="))
print(a+b)
print(b-a)
print(b%a)
print(b**2)
print(b**(1/2))#square root:






enter a-1
enter b=23
24
22
0
529
4.795831523312719




In [25]:



string="BhanuPrakashJha\n"
string[3:7]





Out[25]:

'nuPr'



In [26]:



print(string*5)






BhanuPrakashJha
BhanuPrakashJha
BhanuPrakashJha
BhanuPrakashJha
BhanuPrakashJha





In [37]:



h="HELLO WORLD"
h[::-1]





Out[37]:

'DLROW OLLEH'



In [36]:



St1="I am student"
print(St1[5:8])






stu




In [42]:



a=6
b=7
c=8
print((a+b)**(b-c)/a)






0.012820512820512822



Out[42]:

0.012820512820512822



In [46]:



a=12
print(str(a))






12




In [52]:



St1[0:3]





Out[52]:

'I a'






lab3#16-jan-2020 #Operators



In [10]:



a=10
b=3
print(a//b)
print(a**b)
print(a%b)






3
1000
1




In [12]:



t=325
print(t//60)#min
print(t%60)#sec






5
25




In [26]:



print(a|b)
print(a&b)
print(a^b)
print(~b)






2
2
0
-3




In [23]:



print(a is b)
print(a is not b)
a=2
b=2
print(a is b)
print(a is not b)






True
False
True
False




In [1]:



print(7>>2)
print(10<<2)






1
40




In [5]:



s="I am a student"
print(s)






I am a student




In [3]:



a="abcdefghijklmnopqrstuvwxyz"
a[7:15:2]





Out[3]:

'hjln'



In [1]:



money=eval(input("how much Money you have="))
person=eval(input("enter the number of person"))
ticketPrice=eval(input("enter ticket price="))
autoCharge=eval(input("enter transportation charge="))
snack=eval(input("enter snack price, that you would have during movie="))
sum=autoCharge+person*ticketPrice+snack
if(money<=sum):
    print("Come Back")
else:
    print("GO")






how much Money you have=800
enter ticket price=400
enter transportation charge=120
enter snack price, that you would have during movie=100
GO







lab3#29/02/2020 #Functions



In [12]:



a=eval(input("enter a"))
b=eval(input("enter b"))
c=eval(input("enter c"))
def fun(a,b,c):
    if(a>b and a>c):
        print(a," is greater")
    elif(b>a and b>c):

        print(b," is greater")
    else:
        print(c,"is greater")
fun(a,b,c)






enter a1
enter b2
enter c3
3 is greater




In [24]:



n=eval(input("enter range of list"))
lst=[]
for i in range(n):
    number=eval(input("enter list elements"))
    lst.append(number)

def s(var):
    sz=0
    for i in var:
        sz=sz+i
    return sz
print("sum=",s(lst))






enter range of list4
enter list elements1
enter list elements2
enter list elements3
enter list elements4
sum= 10




In [35]:



str=input("enter String:-")
def ss(str):
    lower=0
    upper=0
    for i in str:
        if(ord(i)>=97 and ord(i)<=120):
            lower+=1
        else:
            upper+=1
    print("Upper=",upper)
    print("Lower=",lower)
ss(str)






enter String:-BhanuPrakashJha
Upper= 3
Lower= 12




In [1]:



a=eval(input("enter num"))
def fz(a):
    n=0
    for i in range(1,a):
        if(a%i==0):
            n=n+i
    if(n==a):
        print(a,"num is perfect")
    else:
        print(a,"is not perfect")
fz(a)






enter num23
23 is not perfect







lab4 #05/02/2020



In [11]:



import pandas as pd
data=pd.read_excel("11909448.xlsx")
data





Out[11]:





Termid

Regd No

Course

Grade

CA_100

MTT_50

ETT_100

ETP_100

Course_Att

MHRDName

...

CA_2

CA_3

CA_4

Weight

ScholarType

Direction

CourseType

Gender

Medium

ProgramType



0
218192 33349776776 QXDAAG391 A 88.0 NaN NaN 68.0 91.0 Bachelor of Technology in Computer Science and... ... 28.0 4.0 19.0 84 Day Scholar East Theory Male Hindi UG 

1
218192 33349776776 QXDAAG51 B+ 65.0 23.0 72.0 NaN 88.0 Bachelor of Technology in Computer Science and... ... 9.0 10.0 2.0 84 Day Scholar East Theory Male Hindi UG 

2
218192 33349776776 QXDAAG52 A+ 82.0 NaN NaN 88.0 91.0 Bachelor of Technology in Computer Science and... ... 5.0 0.0 0.0 84 Day Scholar East Theory Male Hindi UG 

3
218192 33349776776 QXDAAG53 B 45.0 29.0 49.0 NaN 87.0 Bachelor of Technology in Computer Science and... ... 23.0 0.0 0.0 84 Day Scholar East Theory Male Hindi UG 

4
218192 33349776776 QXDAAG54 C 49.0 10.0 59.0 NaN 83.0 Bachelor of Technology in Computer Science and... ... 7.0 7.0 1.0 84 Day Scholar East Theory Male Hindi UG 

5
218192 33349776776 QXDAAG55 B+ 63.0 NaN NaN 79.0 87.0 Bachelor of Technology in Computer Science and... ... 9.0 19.0 0.0 84 Day Scholar East Theory Male Hindi UG 

6
218192 33349776776 QXDAAG56 B 57.0 17.0 45.0 NaN 93.0 Bachelor of Technology in Computer Science and... ... 7.0 10.0 20.0 84 Day Scholar East Theory Male Hindi UG 

7
218192 33349776776 QXDAAG57 B+ 25.0 38.0 73.0 NaN 88.0 Bachelor of Technology in Computer Science and... ... 10.0 2.0 0.0 84 Day Scholar East Theory Male Hindi UG 

8
218192 33349776776 QXDAAG58 C 27.0 28.0 52.0 NaN 85.0 Bachelor of Technology in Computer Science and... ... 12.0 0.0 0.0 84 Day Scholar East Theory Male Hindi UG 

9
118192 33350776776 EBDHJV144 O 100.0 NaN NaN 94.0 93.0 Bachelor of Technology in Computer Science and... ... 30.0 32.0 9.0 73 Day Scholar West Theory Male English UG 

10
118192 33350776776 EBDHJV145 B 62.0 40.0 59.0 NaN 60.0 Bachelor of Technology in Computer Science and... ... 14.0 0.0 30.0 73 Day Scholar West Theory Male English UG 

11
118192 33350776776 EBDHJV20 O 89.0 44.0 86.0 NaN 94.0 Bachelor of Technology in Computer Science and... ... 66.0 1.0 3.0 73 Day Scholar West Theory Male English UG 

12
118192 33350776776 EBDHJV310 A+ 70.0 34.0 78.0 NaN 86.0 Bachelor of Technology in Computer Science and... ... 5.0 12.0 6.0 73 Day Scholar West Theory Male English UG 

13
118192 33350776776 EBDHJV311 O 89.0 NaN NaN 94.0 94.0 Bachelor of Technology in Computer Science and... ... 13.0 28.0 17.0 73 Day Scholar West Theory Male English UG 

14
118192 33350776776 EBDHJV384 A+ 100.0 40.0 76.0 NaN 79.0 Bachelor of Technology in Computer Science and... ... 0.0 1.0 2.0 73 Day Scholar West Theory Male English UG 

15
118192 33350776776 EBDHJV385 B+ 70.0 37.0 64.0 NaN 53.0 Bachelor of Technology in Computer Science and... ... 1.0 14.0 39.0 73 Day Scholar West Theory Male English UG 

16
118192 33350776776 EBDHJV387 A 52.0 34.0 85.0 NaN 71.0 Bachelor of Technology in Computer Science and... ... 9.0 30.0 11.0 73 Day Scholar West Theory Male English UG 

17
118192 33350776776 EBDHJV649 A 78.0 NaN NaN 84.0 93.0 Bachelor of Technology in Computer Science and... ... 5.0 5.0 0.0 73 Day Scholar West Theory Male English UG 

18
118192 33353776776 FAPEUG144 A+ 92.0 NaN NaN 85.0 100.0 Bachelor of Technology in Computer Science and... ... 71.0 9.0 10.0 96 Hostler East Theory Female Hindi UG 

19
118192 33353776776 FAPEUG145 C 50.0 14.0 53.0 NaN 89.0 Bachelor of Technology in Computer Science and... ... 17.0 14.0 15.0 96 Hostler East Theory Female Hindi UG 

20
118192 33353776776 FAPEUG20 C 42.0 24.0 48.0 NaN 86.0 Bachelor of Technology in Computer Science and... ... 2.0 3.0 8.0 96 Hostler East Theory Female Hindi UG 

21
118192 33353776776 FAPEUG312 B 74.0 12.0 49.0 NaN 80.0 Bachelor of Technology in Computer Science and... ... 52.0 2.0 4.0 96 Hostler East Theory Female Hindi UG 

22
118192 33353776776 FAPEUG385 B 59.0 23.0 34.0 NaN 87.0 Bachelor of Technology in Computer Science and... ... 6.0 6.0 33.0 96 Hostler East Theory Female Hindi UG 

23
118192 33353776776 FAPEUG387 C 39.0 28.0 33.0 NaN 86.0 Bachelor of Technology in Computer Science and... ... 3.0 1.0 7.0 96 Hostler East Theory Female Hindi UG 

24
118192 33353776776 FAPEUG649 B 57.0 NaN NaN 60.0 93.0 Bachelor of Technology in Computer Science and... ... 4.0 14.0 2.0 96 Hostler East Theory Female Hindi UG 

25
118192 33353776776 FAPEUG878 E 78.0 23.0 15.0 NaN 92.0 Bachelor of Technology in Computer Science and... ... 9.0 14.0 42.0 96 Hostler East Theory Female Hindi UG 

26
118191 33358776776 AZJGHX2602 A+ 90.0 NaN 68.0 NaN 100.0 Doctor of Philosophy (Electronics and Communic... ... 35.0 3.0 0.0 75 Hostler West Theory Female Regional Ph.D 

27
118191 33358776776 AZJGHX2603 O 90.0 NaN 80.0 NaN 100.0 Doctor of Philosophy (Electronics and Communic... ... 22.0 8.0 9.0 75 Hostler West Theory Female Regional Ph.D 

28
118191 33358776776 AZJGHX2604 A+ 80.0 NaN NaN NaN 100.0 Doctor of Philosophy (Electronics and Communic... ... 5.0 5.0 20.0 75 Hostler West Theory Female Regional Ph.D 

29
118195 33360776776 PHSJDJ2602 A+ 89.0 NaN 72.0 NaN 93.0 Doctor of Philosophy (Mechanical Engineering) ... 14.0 15.0 21.0 84 Hostler North Theory Male Regional Ph.D 

...
... ... ... ... ... ... ... ... ... ... ... ... ... ... ... ... ... ... ... ... ... 

1619
218192 33633776776 SQIMRA370 A 84.0 42.0 59.0 NaN 88.0 Bachelor of Technology in Electronics and Comm... ... 32.0 0.0 1.0 84 Hostler South Theory Female Hindi UG 

1620
218192 33635776776 WVODHY28 B+ 48.0 34.0 55.0 NaN 95.0 Bachelor of Technology (Computer Science and E... ... 2.0 0.0 4.0 99 Day Scholar East Theory Male Regional UG 

1621
218192 33635776776 WVODHY51 A 80.0 23.0 70.0 NaN 93.0 Bachelor of Technology (Computer Science and E... ... 41.0 11.0 9.0 99 Day Scholar East Theory Male Regional UG 

1622
218192 33635776776 WVODHY52 B+ 80.0 NaN NaN 64.0 93.0 Bachelor of Technology (Computer Science and E... ... 1.0 14.0 0.0 99 Day Scholar East Theory Male Regional UG 

1623
218192 33635776776 WVODHY53 B+ 60.0 20.0 63.0 NaN 93.0 Bachelor of Technology (Computer Science and E... ... 13.0 5.0 6.0 99 Day Scholar East Theory Male Regional UG 

1624
218192 33635776776 WVODHY54 B 75.0 22.0 56.0 NaN 91.0 Bachelor of Technology (Computer Science and E... ... 8.0 17.0 38.0 99 Day Scholar East Theory Male Regional UG 

1625
218192 33635776776 WVODHY55 A 77.0 NaN NaN 72.0 93.0 Bachelor of Technology (Computer Science and E... ... 0.0 9.0 24.0 99 Day Scholar East Theory Male Regional UG 

1626
218192 33635776776 WVODHY56 B 57.0 25.0 48.0 NaN 93.0 Bachelor of Technology (Computer Science and E... ... 2.0 4.0 3.0 99 Day Scholar East Theory Male Regional UG 

1627
218192 33635776776 WVODHY57 A+ 77.0 39.0 76.0 NaN 99.0 Bachelor of Technology (Computer Science and E... ... 31.0 14.0 0.0 99 Day Scholar East Theory Male Regional UG 

1628
218192 33635776776 WVODHY58 B+ 25.0 37.0 68.0 NaN 93.0 Bachelor of Technology (Computer Science and E... ... 0.0 11.0 8.0 99 Day Scholar East Theory Male Regional UG 

1629
218192 33636776776 QXDAAG28 A 74.0 34.0 77.0 NaN 83.0 Bachelor of Technology in Computer Science and... ... 22.0 18.0 1.0 68 Hostler South Theory Male Regional UG 

1630
218192 33636776776 QXDAAG391 A 94.0 NaN NaN 70.0 91.0 Bachelor of Technology in Computer Science and... ... 0.0 0.0 0.0 68 Hostler South Theory Male Regional UG 

1631
218192 33636776776 QXDAAG51 A 75.0 27.0 76.0 NaN 93.0 Bachelor of Technology in Computer Science and... ... 7.0 0.0 0.0 68 Hostler South Theory Male Regional UG 

1632
218192 33636776776 QXDAAG52 A 82.0 NaN NaN 81.0 91.0 Bachelor of Technology in Computer Science and... ... 66.0 0.0 12.0 68 Hostler South Theory Male Regional UG 

1633
218192 33636776776 QXDAAG53 A 80.0 29.0 65.0 NaN 85.0 Bachelor of Technology in Computer Science and... ... 7.0 10.0 0.0 68 Hostler South Theory Male Regional UG 

1634
218192 33636776776 QXDAAG54 C 54.0 19.0 43.0 NaN 79.0 Bachelor of Technology in Computer Science and... ... 21.0 8.0 2.0 68 Hostler South Theory Male Regional UG 

1635
218192 33636776776 QXDAAG55 A 84.0 NaN NaN 67.0 87.0 Bachelor of Technology in Computer Science and... ... 0.0 15.0 14.0 68 Hostler South Theory Male Regional UG 

1636
218192 33636776776 QXDAAG56 B+ 64.0 24.0 52.0 NaN 82.0 Bachelor of Technology in Computer Science and... ... 14.0 6.0 6.0 68 Hostler South Theory Male Regional UG 

1637
218192 33636776776 QXDAAG57 A 47.0 35.0 73.0 NaN 83.0 Bachelor of Technology in Computer Science and... ... 30.0 0.0 5.0 68 Hostler South Theory Male Regional UG 

1638
218192 33636776776 QXDAAG58 B 32.0 40.0 53.0 NaN 60.0 Bachelor of Technology in Computer Science and... ... 6.0 1.0 12.0 68 Hostler South Theory Male Regional UG 

1639
118192 33639776776 QSSXAM20 B+ 58.0 23.0 60.0 NaN 92.0 Bachelor of Technology (Electrical and Electro... ... 0.0 0.0 1.0 95 Day Scholar North Theory Female Hindi UG 

1640
118192 33639776776 QSSXAM21 C 57.0 19.0 28.0 NaN 86.0 Bachelor of Technology (Electrical and Electro... ... 34.0 2.0 4.0 95 Day Scholar North Theory Female Hindi UG 

1641
118192 33639776776 QSSXAM22 E 55.0 13.0 26.0 NaN 91.0 Bachelor of Technology (Electrical and Electro... ... 0.0 23.0 32.0 95 Day Scholar North Theory Female Hindi UG 

1642
118192 33639776776 QSSXAM23 C 56.0 20.0 33.0 NaN 90.0 Bachelor of Technology (Electrical and Electro... ... 14.0 1.0 0.0 95 Day Scholar North Theory Female Hindi UG 

1643
118192 33639776776 QSSXAM24 B 70.0 NaN NaN 30.0 92.0 Bachelor of Technology (Electrical and Electro... ... 7.0 12.0 16.0 95 Day Scholar North Theory Female Hindi UG 

1644
118192 33639776776 QSSXAM25 B 74.0 NaN NaN 50.0 100.0 Bachelor of Technology (Electrical and Electro... ... 18.0 33.0 22.0 95 Day Scholar North Theory Female Hindi UG 

1645
118192 33639776776 QSSXAM26 B+ 72.0 15.0 52.0 NaN 91.0 Bachelor of Technology (Electrical and Electro... ... 32.0 5.0 2.0 95 Day Scholar North Theory Female Hindi UG 

1646
118192 33639776776 QSSXAM27 C 57.0 12.0 46.0 NaN 91.0 Bachelor of Technology (Electrical and Electro... ... 0.0 1.0 2.0 95 Day Scholar North Theory Female Hindi UG 

1647
118192 33639776776 QSSXAM28 A 65.0 27.0 67.0 NaN 92.0 Bachelor of Technology (Electrical and Electro... ... 3.0 7.0 4.0 95 Day Scholar North Theory Female Hindi UG 

1648
118192 33640776776 TVJMWD1480 O 88.0 NaN NaN 97.0 91.0 Bachelor of Science (Honours) (Food Technology) ... 4.0 2.0 1.0 62 Day Scholar South Theory Female English UG 

1649 rows × 22 columns



In [14]:



import matplotlib.pyplot as ptl
a=[10,20,10,60,12]
b=[1,2,3,2,1]
ptl.plot(a,b,linewidth=5,color='r')
ptl.xlabel("xxxx")
ptl.ylabel("yyyy")





Out[14]:

Text(0, 0.5, 'yyyy')



 



In [32]:



z=[5,6,7,8,9,3,6,5,5]
ptl.hist(z)





Out[32]:

(array([1., 0., 0., 3., 0., 2., 1., 0., 1., 1.]),
 array([3. , 3.6, 4.2, 4.8, 5.4, 6. , 6.6, 7.2, 7.8, 8.4, 9. ]),
 <a list of 10 Patch objects>)



 



In [9]:



import pandas as pd
data=pd.read_excel("11909448.xlsx")
ptl.hist(data['CA_100'],bins=100)






C:\Users\Sony\Anaconda3\lib\site-packages\numpy\lib\histograms.py:824: RuntimeWarning: invalid value encountered in greater_equal
  keep = (tmp_a >= first_edge)
C:\Users\Sony\Anaconda3\lib\site-packages\numpy\lib\histograms.py:825: RuntimeWarning: invalid value encountered in less_equal
  keep &= (tmp_a <= last_edge)



Out[9]:

(array([10.,  0.,  0.,  0.,  4.,  2.,  0.,  3.,  0.,  1.,  6.,  0.,  3.,
         1.,  4.,  3.,  0.,  3.,  0.,  3.,  5.,  1.,  6.,  2.,  3., 10.,
         0.,  6.,  1.,  9., 11.,  1., 10.,  3., 10.,  8.,  5., 25.,  4.,
        11., 22., 11., 18.,  7., 24., 22.,  9., 26.,  7., 23., 30.,  9.,
        20., 13., 30., 34., 11., 45., 10., 27., 27., 12., 45., 16., 44.,
        60.,  9., 43., 14., 24., 43., 23., 46., 19., 45., 47., 20., 30.,
        23., 43., 63.,  8., 42., 12., 39., 28.,  9., 28., 11., 33., 32.,
         7., 26., 10., 25., 14., 10.,  9.,  5., 25.]),
 array([  0.,   1.,   2.,   3.,   4.,   5.,   6.,   7.,   8.,   9.,  10.,
         11.,  12.,  13.,  14.,  15.,  16.,  17.,  18.,  19.,  20.,  21.,
         22.,  23.,  24.,  25.,  26.,  27.,  28.,  29.,  30.,  31.,  32.,
         33.,  34.,  35.,  36.,  37.,  38.,  39.,  40.,  41.,  42.,  43.,
         44.,  45.,  46.,  47.,  48.,  49.,  50.,  51.,  52.,  53.,  54.,
         55.,  56.,  57.,  58.,  59.,  60.,  61.,  62.,  63.,  64.,  65.,
         66.,  67.,  68.,  69.,  70.,  71.,  72.,  73.,  74.,  75.,  76.,
         77.,  78.,  79.,  80.,  81.,  82.,  83.,  84.,  85.,  86.,  87.,
         88.,  89.,  90.,  91.,  92.,  93.,  94.,  95.,  96.,  97.,  98.,
         99., 100.]),
 <a list of 100 Patch objects>)



 



In [38]:



labels=["a","b","c","d"]
sizes=[100,200,300,400]
explode=[0,.3,0,0]
colors = ['yellowgreen', 'gold', 'lightskyblue', 'lightcoral']
ptl.pie(sizes,labels=labels,colors=colors,shadow='true',explode=explode,autopct='%1.1f%%')





Out[38]:

([<matplotlib.patches.Wedge at 0x1fefc8df9e8>,
  <matplotlib.patches.Wedge at 0x1fefc8ec400>,
  <matplotlib.patches.Wedge at 0x1fefc8ecd30>,
  <matplotlib.patches.Wedge at 0x1fefc8f86a0>],
 [Text(1.0461621663333946, 0.3399186987098808, 'a'),
  Text(0.4326237671925118, 1.3314791309142473, 'b'),
  Text(-1.0461621902025062, 0.3399186252483017, 'c'),
  Text(0.3399188211458418, -1.0461621265515308, 'd')],
 [Text(0.5706339089091244, 0.1854101992962986, '10.0%'),
  Text(0.27811527890947185, 0.8559508698734446, '20.0%'),
  Text(-0.5706339219286397, 0.18541015922634638, '30.0%'),
  Text(0.18541026607955005, -0.5706338872099259, '40.0%')])



 



In [49]:



import matplotlib.pyplot as plt
import pandas as pd
data=pd.read_excel("11909448.xlsx")
i=data['Grade']
a=0
b=0
c=0
e=0
for z in i[:]:
    if z=='A+' or z=='A' or z=='O':
        a=a+1
    elif z=='B+' or z=='B':
        b=b+1
    elif z=='C' or z=='D':
        c=c+1
    elif z=='E':
        e=e+1
labels=["O, A, A+","B+, B","C, D","E"]
sizes=[a,b,c,e]
explode=[0,0,0,0.3]
colors = ['yellowgreen', 'gold', 'lightskyblue', 'lightcoral']
plt.pie(sizes,labels=labels,colors=colors,shadow='true',autopct='%1.1f%%',explode=explode)





Out[49]:

([<matplotlib.patches.Wedge at 0x1aba10b4470>,
  <matplotlib.patches.Wedge at 0x1aba23505c0>,
  <matplotlib.patches.Wedge at 0x1aba2343748>,
  <matplotlib.patches.Wedge at 0x1aba22a0128>],
 [Text(0.41530359930341787, 1.0185886904956418, 'O, A, A+'),
  Text(-1.0313010564619707, -0.38264622164660544, 'B+, B'),
  Text(0.45432045430630563, -1.0017948516532276, 'C, D'),
  Text(1.3303890246496426, -0.43596449751301214, 'E')],
 [Text(0.22652923598368244, 0.555593831179441, '37.7%'),
  Text(-0.5625278489792567, -0.2087161208981484, '36.0%'),
  Text(0.2478111568943485, -0.546433555447215, '16.3%'),
  Text(0.8552500872747701, -0.28026289125836495, '10.1%')])



 



In [73]:



import numpy as np
col=data['ProgramType']
ug=0
phd=0
pg=0
for i in col[:]:
    if i=='UG':
        ug+=1
    elif i=='Ph.D':
        phd+=1
    else:
        pg+=1
languages=('ug','pg','phd')
y_pos=np.arange(len(languages))
performance=[ug,pg,phd]
plt.bar(y_pos,performance)
plt.xticks(y_pos,languages)
plt.show()
print(phd)
print(ug)
print(pg)
data.ProgramType.value_counts()






 



26
1556
67



Out[73]:

UG      1556
PG        67
Ph.D      26
Name: ProgramType, dtype: int64



In [80]:



x=data.Height.value_counts()
plt.boxplot(x)
y=data.Weight.value_counts()
data.Medium.value_counts()





Out[80]:

Hindi       620
English     531
Regional    498
Name: Medium, dtype: int64



 



In [20]:



a='Bhanu Prakash'
a[0:]
a[:3]
a[0:3]
a[4::-1]
a[-3::]





Out[20]:

'ash'



In [41]:



class Animal:
    nol=4
dog=Animal()
dog.nol

class Bp:
    m=10
    def add(self,a,b):
        t=a+b
        print(t)
        
b=Bp()
b.add(3,4)
print(Bp.m)






7
10




In [1]:



class Student:
    name="Bhanu"
    rollNo=1




In [21]:



import math
class Circle:
    def __init__(self,r):
        self.r=r
    def get_area(self):
        return 2*math.pi*self.r**2
    def get_circum(self):
        return 2*math.pi*self.r
c=Circle(10)
print(c.get_area())
print(c.get_circum())






628.3185307179587
62.83185307179586




In [15]:



class Temp:
    def celsius(self,cl):
        self.cl=cl
        t=cl*1.8+32
        return t
    def Fahrenheit(self,fa):
        self.fa=fa
        t=(fa-32)/1.8
        return t
t=Temp()
ip=eval(input("Enter 1 for C to F \n2 for F to C"))
if(ip==1):
    h=eval(input("enter celsius "))
    print(t.celsius(h),"F")
elif(ip==2):
    j=eval(input("enter Fahrenheit "))
    print(t.Fahrenheit(j),"C")
else:
    print("Select Right Option")






Enter 1 for C to F 
2 for F to C4
Select Right Option




In [1]:



import tensorflow as tf
from tensorflow import keras




In [15]:



print ("TensorFlow version: " + tf.__version__)
tf.compat.v1.disable_eager_execution()
sess = tf.compat.v1.Session()






TensorFlow version: 2.1.0




In [16]:



c1=tf.constant(10)
c2=tf.constant("asdf")
tf.compat.v1.disable_eager_execution()
sess = tf.compat.v1.Session()
sess.run([c1,c2])





Out[16]:

[10, b'asdf']






Covid-19



In [125]:



import requests
from pandas.io.json import json_normalize
URL = "https://api.covid19india.org/data.json"
data = requests.get(url=URL).json()
covid19_df = json_normalize(data['statewise'])
print("Total Confirmed Cases: "+str(covid19_df[covid19_df.state == "Total"]['confirmed']))
print("Total Active Cases: "+str(covid19_df[covid19_df.state == "Total"]['active']))
print("Total Recovered Cases: "+str(covid19_df[covid19_df.state == "Total"]['recovered']))
print("Total Deceased Cases: "+str(covid19_df[covid19_df.state == "Total"]['deaths']))
print(covid19_df[['state','confirmed','active','recovered','deaths']].sort_values(by="confirmed", ascending=False))






Total Confirmed Cases: 0    14352
Name: confirmed, dtype: object
Total Active Cases: 0    11825
Name: active, dtype: object
Total Recovered Cases: 0    2041
Name: recovered, dtype: object
Total Deceased Cases: 0    486
Name: deaths, dtype: object
                          state confirmed active recovered deaths
26                    Meghalaya         9      8         0      1
16                        Bihar        85     47        37      1
7                 Uttar Pradesh       849    753        82     14
8                     Telangana       766    561       187     18
28                   Puducherry         7      6         1      0
27                          Goa         7      1         6      0
17                       Odisha        60     38        21      1
9                Andhra Pradesh       572    523        35     14
18                  Uttarakhand        40     31         9      0
10                       Kerala       395    138       255      2
20             Himachal Pradesh        38     20        16      2
19                 Chhattisgarh        36     12        24      0
11                    Karnataka       359    258        88     13
21                        Assam        34     24         9      1
1                   Maharashtra      3320   2788       331    201
12            Jammu and Kashmir       328    281        42      5
22                    Jharkhand        32     30         0      2
13                  West Bengal       255    194        51     10
14                      Haryana       223    134        86      3
15                       Punjab       211    167        30     14
23                   Chandigarh        21     12         9      0
29                      Manipur         2      1         1      0
30                      Tripura         2      1         1      0
24                       Ladakh        18      4        14      0
2                         Delhi      1707   1593        72     42
0                         Total     14352  11825      2041    486
3                    Tamil Nadu      1323   1025       283     15
5                Madhya Pradesh      1310   1171        70     69
4                     Rajasthan      1229   1029       183     17
25  Andaman and Nicobar Islands        12      1        11      0
6                       Gujarat      1099    972        86     41
31                      Mizoram         1      1         0      0
32            Arunachal Pradesh         1      0         1      0
33                     Nagaland         1      1         0      0
34       Dadra and Nagar Haveli         0      0         0      0
35                Daman and Diu         0      0         0      0
36                  Lakshadweep         0      0         0      0
37                       Sikkim         0      0         0      0




In [126]:



covid19_df





Out[126]:





active

confirmed

deaths

deltaconfirmed

deltadeaths

deltarecovered

lastupdatedtime

recovered

state

statecode

statenotes



0
11825 14352 486 920 38 273 18/04/2020 00:45:05 2041 Total TT  

1
2788 3320 201 118 7 31 17/04/2020 23:45:05 331 Maharashtra MH  

2
1593 1707 42 67 4 20 17/04/2020 21:52:06 72 Delhi DL  

3
1025 1323 15 56 0 103 17/04/2020 18:55:06 283 Tamil Nadu TN  

4
1029 1229 17 98 6 19 17/04/2020 21:49:07 183 Rajasthan RJ  

5
1171 1310 69 146 14 0 17/04/2020 20:15:10 70 Madhya Pradesh MP  

6
972 1099 41 170 5 13 17/04/2020 20:15:11 86 Gujarat GJ  

7
753 849 14 44 1 14 17/04/2020 20:37:09 82 Uttar Pradesh UP  

8
561 766 18 66 0 0 17/04/2020 20:15:12 187 Telangana TG  

9
523 572 14 38 0 15 17/04/2020 11:53:06 35 Andhra Pradesh AP  

10
138 395 2 1 0 10 17/04/2020 18:14:06 255 Kerala KL  

11
258 359 13 44 0 6 17/04/2020 17:46:06 88 Karnataka KA  

12
281 328 5 14 1 4 17/04/2020 20:04:08 42 Jammu and Kashmir JK  

13
194 255 10 24 0 9 17/04/2020 08:43:06 51 West Bengal WB As WB state bulletin only reports the number o... 

14
134 223 3 8 0 21 17/04/2020 19:25:09 86 Haryana HR 14 recovered Italian tourists included in tall... 

15
167 211 14 14 0 1 17/04/2020 18:55:29 30 Punjab PB  

16
47 85 1 2 0 0 18/04/2020 00:45:06 37 Bihar BR  

17
38 60 1 0 0 2 17/04/2020 20:37:11 21 Odisha OR  

18
31 40 0 3 0 0 17/04/2020 17:46:07 9 Uttarakhand UT  

19
12 36 0 0 0 1 17/04/2020 19:15:07 24 Chhattisgarh CT  

20
20 38 2 3 0 0 18/04/2020 00:45:07 16 Himachal Pradesh HP Death of Tibetan refugee included 

21
24 34 1 0 0 4 18/04/2020 00:25:07 9 Assam AS  

22
30 32 2 3 0 0 17/04/2020 21:09:07 0 Jharkhand JH  

23
12 21 0 0 0 0 15/04/2020 17:20:25 9 Chandigarh CH  

24
4 18 0 0 0 0 16/04/2020 15:13:07 14 Ladakh LA  

25
1 12 0 1 0 0 16/04/2020 16:53:07 11 Andaman and Nicobar Islands AN  

26
8 9 1 0 0 0 16/04/2020 23:43:08 0 Meghalaya ML  

27
1 7 0 0 0 0 15/04/2020 20:10:36 6 Goa GA  

28
6 7 0 0 0 0 10/04/2020 17:50:26 1 Puducherry PY  

29
1 2 0 0 0 0 06/04/2020 22:35:54 1 Manipur MN  

30
1 2 0 0 0 0 10/04/2020 20:00:27 1 Tripura TR  

31
1 1 0 0 0 0 26/03/2020 07:19:29 0 Mizoram MZ  

32
0 1 0 0 0 0 16/04/2020 19:33:11 1 Arunachal Pradesh AR  

33
1 1 0 0 0 0 12/04/2020 23:35:29 0 Nagaland NL  

34
0 0 0 0 0 0 17/04/2020 15:03:07 0 Dadra and Nagar Haveli DN  

35
0 0 0 0 0 0 26/03/2020 07:19:29 0 Daman and Diu DD  

36
0 0 0 0 0 0 26/03/2020 07:19:29 0 Lakshadweep LD  

37
0 0 0 0 0 0 26/03/2020 07:19:29 0 Sikkim SK  



In [34]:



active=covid19_df['active'][0]
confirmed=covid19_df['confirmed'][0]
deltaconfirmed=covid19_df['deltaconfirmed'][0]
deaths=covid19_df['deaths'][0]
deltadeaths=covid19_df['deltadeaths'][0]
recovered=covid19_df['recovered'][0]
deltarecovered=covid19_df['deltarecovered'][0]




In [53]:



import numpy as np
import matplotlib.pyplot as plt
import pandas as pd
title=('active','confirmed','deltaconfirmed','deaths','deltadeaths','recovered','deltarecovered')
y_pos=np.arange(len(title))
performance=[active,confirmed,deltaconfirmed,deaths,deltadeaths,recovered,deltarecovered]
#plt.plot([active,confirmed,deltaconfirmed,deaths,deltadeaths,recovered,deltarecovered])




In [ ]:



# import matplotlib.pyplot as plt 
  
# x-axis values 
x = ['act','conf','dconf','de','dde','rec','drec'] 
# y-axis values 
y = [active,confirmed,deltaconfirmed,deaths,deltadeaths,recovered,deltarecovered] 
  
# plotting points as a scatter plot 
plt.scatter(x, y, label= "stars", color= "green",  
            marker= "*", s=30) 
  
# x-axis label 
plt.xlabel('x - axis') 
# frequency label 
plt.ylabel('y - axis') 
# plot title 
plt.title('My scatter plot!') 
# showing legend 
plt.legend() 
  
# function to show the plot 
plt.show() 
print('act = Total Active Cases')
print('cnf = Total Confirmed cases')
print('dconf = Total Deltaconfirmed cases')
print('de = Total Deaths')
print('dde = Total Deltadeaths')
print('rec = Total Recovered')
print('drec = Total Deltarecovered')







ScatterPlot



In [78]:



import matplotlib.pyplot as plt 
import requests
from pandas.io.json import json_normalize
URL = "https://api.covid19india.org/data.json"
data = requests.get(url=URL).json()
covid19_df = json_normalize(data['statewise']) 
active=covid19_df['active'][0]
confirmed=covid19_df['confirmed'][0]
deltaconfirmed=covid19_df['deltaconfirmed'][0]
deaths=covid19_df['deaths'][0]
deltadeaths=covid19_df['deltadeaths'][0]
recovered=covid19_df['recovered'][0]
deltarecovered=covid19_df['deltarecovered'][0]

# x-axis values 
x = ['act','conf','dconf','de','dde','rec','drec'] 
# y-axis values 
y = [active,confirmed,deltaconfirmed,deaths,deltadeaths,recovered,deltarecovered] 
  
# plotting points as a scatter plot 
plt.scatter(x, y, label= "stars", color= "green",  
            marker= "*", s=30) 
  
# x-axis label 
plt.xlabel('x - axis') 
# frequency label 
plt.ylabel('y - axis') 
# plot title 
plt.title('My scatter plot!') 
# showing legend 
plt.legend() 
  
# function to show the plot 
plt.show() 
print('act = Total Active Cases')
print('cnf = Total Confirmed cases')
print('dconf = Total Deltaconfirmed cases')
print('de = Total Deaths')
print('dde = Total Deltadeaths')
print('rec = Total Recovered')
print('drec = Total Deltarecovered')






 



act = Total Active Cases
cnf = Total Confirmed cases
dconf = Total Deltaconfirmed cases
de = Total Deaths
dde = Total Deltadeaths
rec = Total Recovered
drec = Total Deltarecovered







pie chart



In [147]:



import matplotlib.pyplot as plt 
import requests
from pandas.io.json import json_normalize
URL = "https://api.covid19india.org/data.json"
data = requests.get(url=URL).json()
covid19_df = json_normalize(data['statewise']) 
active=covid19_df['active'][0]
confirmed=covid19_df['confirmed'][0]
deltaconfirmed=covid19_df['deltaconfirmed'][0]
deaths=covid19_df['deaths'][0]
deltadeaths=covid19_df['deltadeaths'][0]
recovered=covid19_df['recovered'][0]
deltarecovered=covid19_df['deltarecovered'][0]


labels=['death','Deltadeaths','Recoverd','TotalRecovered']
sizes=[deaths,deltadeaths,recovered,deltarecovered]
explode=[0.2,0.3,0,0]
colors = ['orange','red','lightblue','pink']
plt.figure(figsize = (10, 7))
plt.pie(sizes,labels=labels,colors=colors,shadow='true',autopct='%1.1f%%',explode=explode,startangle=90)





Out[147]:

([<matplotlib.patches.Wedge at 0x23067b96b70>,
  <matplotlib.patches.Wedge at 0x23068dc6080>,
  <matplotlib.patches.Wedge at 0x23068dc64e0>,
  <matplotlib.patches.Wedge at 0x230670b62b0>],
 [Text(-0.6661336424633277, 1.116362830973219, 'death'),
  Text(-1.258945096102671, 0.6124191742581524, 'Deltadeaths'),
  Text(0.30171818621799495, -1.0578119568738686, 'Recoverd'),
  Text(0.3273874729819897, 1.0501511522321285, 'TotalRecovered')],
 [Text(-0.40992839536204784, 0.6869925113681346, '17.1%'),
  Text(-0.809321847494574, 0.3936980405945265, '1.3%'),
  Text(0.16457355611890634, -0.5769883401130192, '71.9%'),
  Text(0.17857498526290347, 0.5728097193993428, '9.6%')])



 






Num of death state wise : line plot



In [221]:



import matplotlib.pyplot as plt 
import requests
import numpy as np
from pandas.io.json import json_normalize
URL = "https://api.covid19india.org/data.json"
data = requests.get(url=URL).json()
covid19_df = json_normalize(data['statewise'])
statename=[]
ideath=[]
for i in covid19_df['statecode'][1:]:
    statename.append(i)
for i in covid19_df['deaths'][1:]:
    ideath.append(i)
    
plt.figure(figsize = (12, 7))
plt.plot(statename, ideath)
plt.show()
import itertools 
for (a,b) in zip(covid19_dfnew['statecode'], covid19_dfnew['state']):
    print(a , ' = ' , b)






 



MH  =  Maharashtra
DL  =  Delhi
TN  =  Tamil Nadu
RJ  =  Rajasthan
MP  =  Madhya Pradesh
GJ  =  Gujarat
UP  =  Uttar Pradesh
TG  =  Telangana
AP  =  Andhra Pradesh
KL  =  Kerala
KA  =  Karnataka
JK  =  Jammu and Kashmir
WB  =  West Bengal
HR  =  Haryana
PB  =  Punjab
BR  =  Bihar
OR  =  Odisha
UT  =  Uttarakhand
CT  =  Chhattisgarh
HP  =  Himachal Pradesh
AS  =  Assam
JH  =  Jharkhand
CH  =  Chandigarh
LA  =  Ladakh
AN  =  Andaman and Nicobar Islands
ML  =  Meghalaya
GA  =  Goa
PY  =  Puducherry
MN  =  Manipur
TR  =  Tripura
MZ  =  Mizoram
AR  =  Arunachal Pradesh
NL  =  Nagaland
DN  =  Dadra and Nagar Haveli
DD  =  Daman and Diu
LD  =  Lakshadweep
SK  =  Sikkim







Bar Plot



In [174]:



import matplotlib.pyplot as plt 
import requests
from pandas.io.json import json_normalize
URL = "https://api.covid19india.org/data.json"
data = requests.get(url=URL).json()
covid19_df = json_normalize(data['statewise']) 

active=covid19_df['active'][0]
confirmed=covid19_df['confirmed'][0]
deltaconfirmed=covid19_df['deltaconfirmed'][0]
deaths=covid19_df['deaths'][0]
deltadeaths=covid19_df['deltadeaths'][0]
recovered=covid19_df['recovered'][0]
deltarecovered=covid19_df['deltarecovered'][0]
time=covid19_df['lastupdatedtime'][0]
# x-coordinates of left sides of bars  
left = [1,2,3,4,5,6,7] 
  
# heights of bars 
height = [active,confirmed,deltaconfirmed,deaths,deltadeaths,recovered,deltarecovered] 
  
# labels for bars 
tick_label = ['active','confirmed','deltaconfirmed','deaths','deltadeaths','recovered','deltarecovered'] 
plt.figure(figsize = (12, 7))
# plotting a bar chart 
plt.bar(left, height, tick_label = tick_label, 
        width = 0.8, color = ['red', 'green']) 

# naming the x-axis 
plt.xlabel('x - axis') 
# naming the y-axis 
plt.ylabel('y - axis') 
# plot title 
plt.title('Covid-19') 

plt.show() 
print('last updated time = ' , time)






 



last updated time =  18/04/2020 10:14:05







Area Plot:-



In [192]:



import matplotlib.pyplot as plt 
import requests
from pandas.io.json import json_normalize
URL = "https://api.covid19india.org/data.json"
data = requests.get(url=URL).json()
covid19_df = json_normalize(data['statewise']) 
covid19_dfnew=covid19_df.drop(covid19_df.index[[0]])
count=[1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31,32,33,34,35,36,37]

active =covid19_dfnew['active']
confirmed=covid19_dfnew['confirmed']
recovered =covid19_dfnew['recovered']
deaths = covid19_dfnew['deaths']
plt.figure(figsize = (12, 7))
plt.plot([],[],color='m', label='active', linewidth=5)
plt.plot([],[],color='c', label='confirmed', linewidth=5)
plt.plot([],[],color='r', label='recovered', linewidth=5)
plt.plot([],[],color='k', label='deaths', linewidth=5)
  
plt.stackplot(count, active,confirmed,recovered,deaths, colors=['m','c','r','k'])
plt.xlabel('x')
plt.ylabel('y')
plt.title('Stack Plot')
plt.legend()
plt.show()






 






Line Plot - Deaths and Recovered



In [223]:



import matplotlib.pyplot as plt 
import requests
from pandas.io.json import json_normalize
URL = "https://api.covid19india.org/data.json"
data = requests.get(url=URL).json()
covid19_df = json_normalize(data['statewise']) 
covid19_dfnew=covid19_df.drop(covid19_df.index[[0]])
plt.figure(figsize = (12, 7))
statecode=covid19_dfnew['statecode']
recovered=covid19_dfnew['recovered']
deaths=covid19_dfnew['deaths']
plt.plot(statecode, recovered, label='covid-19')
plt.plot(statecode, deaths, label='covid-19')
import itertools 
for (a,b) in zip(covid19_dfnew['statecode'], covid19_dfnew['state']):
    print(a , ' = ' , b)






MH  =  Maharashtra
DL  =  Delhi
TN  =  Tamil Nadu
RJ  =  Rajasthan
MP  =  Madhya Pradesh
GJ  =  Gujarat
UP  =  Uttar Pradesh
TG  =  Telangana
AP  =  Andhra Pradesh
KL  =  Kerala
KA  =  Karnataka
JK  =  Jammu and Kashmir
WB  =  West Bengal
HR  =  Haryana
PB  =  Punjab
BR  =  Bihar
OR  =  Odisha
UT  =  Uttarakhand
CT  =  Chhattisgarh
HP  =  Himachal Pradesh
AS  =  Assam
JH  =  Jharkhand
CH  =  Chandigarh
LA  =  Ladakh
AN  =  Andaman and Nicobar Islands
ML  =  Meghalaya
GA  =  Goa
PY  =  Puducherry
MN  =  Manipur
TR  =  Tripura
MZ  =  Mizoram
AR  =  Arunachal Pradesh
NL  =  Nagaland
DN  =  Dadra and Nagar Haveli
DD  =  Daman and Diu
LD  =  Lakshadweep
SK  =  Sikkim




 



In [ ]:



 

