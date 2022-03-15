# Tequed-labs
python based AI ML
'''qw = [1, 12, 'huzair']
print(qw)
for i in list:
  print(i)'''
# print(qw.)

# set- {}

'''s = {1,2,4,5,4,675}
b = {1, 3, 44, 6}
print(type(s))
print(s)
# union
s | b

#intersection
s & b'''

# dictionary

'''d = {1:'ONE', 2:'tWO', 3:"three"}
b = {'tata':'unordered','no':'no is num py' }
print(d)
print(b)
print(d[1])
print(d.values())
print(d.keys())'''

#num py is list, faster and efficient
# sometimes list will be slow if data is large

import numpy as np
'''a = np.array(1)
print(a)
print(type(a))

# array(1)
print(a.ndim) #it is a scalar 0 dimension and 1 d is vector
print(a.shape)
b = np.array([1,2, 4, 5])
print(b)
b
b.ndim
b.shape'''

'''c = np.array([[1,2,3], [7, 8,9]])
c.shape
c.ndim
print(c.shape)'''

# package is collection of librwary
# import random
'''d = np.random.randint(0,10,10)
print(d)
d.size
d.shape
d.ndim
d=d.reshape(2, 5)
print(d)
print(d.shape)
print(d.dtype)
d.astype('float32')'''

'''x = np.ones(10)
x.dtype

y = np.zeros(5)
y

z = np.zeros([3,3]) #3 rows, 3 columns
z
z.shape
k = np.random.randint(1,10,size= (3,3))
k'''

x = np.array(['apple','mando', 'Grapes', 'orange'])
x

y = np.array([25, 'apple', '3.0', 3.0, True, None ])
y

a = np.array([1,2,3,4])

# index part

a[0]
a[1:3]

# scaling /normalization
# we are checking as to how normalization works

'''import numpy as np
import matplotlib.pyplot as plt
np.random.seed(0)  # make constant values with random by seed

x1 = np.random.randint(1,50,30)
x1= np.sort(x1)
x2 = np.random.randint(10000, 70000, 30)
plt.plot(x1,x2)
# x2 =  after normallization

x1min = min(x1)
x1max = max(x1)
x2min = min(x2)
x2max = max(x2)
x1norm = (x1- x1min)/(x1max-x1min)
x2norm = (x2- x2min)/(x2max-x2min)
plt.plot(x1norm, x2norm)
'''

# visualization library - matplotlib
'''import matplotlib.pyplot as plt
i = np.array([[[87,255,205]]])  #black 000 white - 111 255,255,255
plt.imshow(i)
pallet = np.array([[0,0,0],[0,255,50],[0,100,30]])
i = np.array([[0,1,2]])
plt.imshow(pallet[i])


x = [1,2,4]
y= [5,67,8]
plt.plot(x,y, c='r', marker='.')
Marker	Description
“.”	point
“, “	pixel
“o”	circle
“v”	triangle_down
“^”	triangle_up
“<“	triangle_left
“>”	triangle_right
“1”	tri_down
“2”	tri_up
“3”	tri_left
“4”	tri_right
“8”	octagon
“s”	square
“p”	pentagon
“P”	plus (filled)
“*”	star
“h”	hexagon1
“H”	hexagon2
“+”	plus
“x”	x
“X”	x (filled)
“D”	diamond
“d”	thin_diamond
“|”	vline
“_”	hline
plt.title('x- axis')
plt.xlabel('x- axis')
plt.ylabel('y- axis')'''

'''import matplotlib.pyplot as plt
x = [1,9,1]
y= [5,67,5]
plt.title('GRAPH')
plt.xlabel('x- axis')
plt.ylabel('y- axis')
plt.plot(x,y, c='r', marker='p', linewidth = '4')   '''

# analysis
'''overs = [0,4,8,16,20]
team1= [1,7,4,13,5]
team2= [5,13,3,4,18]
plt.title("analysis of cricket match")
plt.plot(overs,team1, label='TEam1')
plt.plot(overs,team2, label='TEam2')
plt.xlabel("overs")
plt.ylabel("score")
plt.legend()'''

# data
import matplotlib.pyplot as plt
x = [60,70,80,90,100]
y = np.array([250,270,269,280,300])
plt.plot(x,y)
plt.title("sports data")
plt.xlabel("avg pluse")
plt.ylabel("calories")
plt.grid()

#subplot
fig= plt.figure()

x1 = np.random.randint(0,10,5)
x2 = np.random.randint(0,10,5)
y1 = np.random.randint(0,10,5)
y2 = np.random.randint(0,10,5)

ax1 = fig.add_subplot(221)
ax2 = fig.add_subplot(224)
ax1.plot(x1,y1)
ax1.plot(x2,y1)

#scatter plot
a=[1,2,3,4,54]
b=[2,3,4,5,6]
plt.title('scatter plot')
plt.scatter(a,b)
