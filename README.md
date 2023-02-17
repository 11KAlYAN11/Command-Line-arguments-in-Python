# Command-Line-arguments-in-Python


Date 28/08/2022

Command Line arguments

1)
'''import sys
print(type(sys.argv))# here o/p is class<list> bcz argv is not a array it is a list
print(sys.argv[0])'''

"""from sys import argv
print("Length of argv: ",len(argv))
print("List of command line arguments: ",argv)
for i in argv:
    print(i)"""


from sys import argv 
print("Length of arguments: ",len(argv))
print("Command Line Arguments: ",argv)
print("Commands Line argumenets one by one")
for i in argv:
    print(i)



o/p:PS D:\Ka_VS_CoDe\K@ly@N> py practice11.py 10 20 30 40 50 #HERE clearely observe that first plave py nameofthefile inc with.py ** py kalyan.py**
Length of arguments:  6
Command Line Arguments:  ['practice11.py', '10', '20', '30', '40', '50']
Commands Line argumenets one by one
practice11.py
10
20
30
40
50


2)

for i in range(1,n+1):
    #ele= int(input())
    l.append(int(input()))

print(l)

o/p:
4
1
2
3
4
[1, 2, 3, 4]

1
4



3)
x,y,z = map(int,input("Enter 3 numbers: ").split())
print(x,y,z)

o/p:
10 20 30



n = 10
l = list(map(int,input().split()))[:n]  #[0:n]   #by default index starts from zero only
print(l)

#takeing n items into a list
o/p:
n = 10
1 2 3 4 5 6 7 8 9 10
[1, 2, 3, 4, 5, 6, 7, 8, 9, 10]




n = int(input())
l = list(map(int,input().strip().split()))[:n]  #[0:n]   #by default index starts from zero only
print(l)#.strip used to cover unexpected spaces 



name=""
while name != "kalyan":
    name = input("Enter name: ")
print("Thanks for conformation!..")

o/p:Enter name: asam
Enter name: pandu
Enter name: reddy
Enter name: kalyan
Thanks for conformation!..

o/p2:
Enter name: asam
Enter name: reddy
Enter name: pandu 
Enter name: master
Enter name: developer
Enter name: loverboy
Enter name: intelligent
Enter name: all rounder
Enter name: specialist
Enter name: kalyan
Thanks for conformation!..


4)
import math
for i in range(1,100+1):
    for j in range(2,int(i/2)):
        if(i%j == 0):
            break
    else:
        print(i,end='  ')

o/p:
1  2  3  4  5  7  11  13  17  19  23  29  31  37  
41  43  47  53  59  61  67  71  73  79  83  89  97

EXP: here else is nothing but loop w/o break, if break not executed in loop then else will be executed
above prime number program is example for that

**else means loop Without break**


