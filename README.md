# Write a function to print the times table of a given number
def tables(n):
    for i in range(1,11):
        print(i,'*',n,'=',n*i)

# whether the string is palindrome or not
def palindrome(str1):
    for i in range(0,len(str1)):
        if str1[i]==str1[len(str1)-i-1]:
            return True
        return False
result=palindrome("mars")
if(result):
   print("yes,the string is palindrome")
else:
    print("no,the string is not a palindrome")


# write a program to print 1 to n ,fizz for multiples of 3,buzz for multiples of 5 and fizzbuzz for multiples of 15
def fizbuz(n):
    for i in range(1,n):
        if(i%15==0):
            print("fizzbuzz")
            continue
        elif(i%3==0):
            print("fizz")
            continue
        elif(i%5==0):
            print("buzz")
            continue
        print(i)

# program to check whether the string is a panagram or not
def pangram_1(string):
    for i in "abcdefghijklmnopqrstuvwxyz":
        if i not in string.lower():
            return False
        return True
result=pangram_1("the quick brown fox jumps over the dog")
if result==True:
    print("pangram")
else:
    print("not pangram")

            
# map routine to produce a list of sqaure of numbers
list1=[1,2,3,4,5,6,7,8,9,10]
square=(list(map(lambda i:i**2,list1)))
print(square)

# reverse the key/value relationship of a dictionary
dict1={"gujarat":"gandhinagar","meghalaya":"shillong"}
print(dict1)
rev={v:k for k,v in dict1.items()}
print(rev)

# Write a program to find prime factors of a given number 
import math
def primefac(n):
    while n%2==0:
        print("2")
        n=n//2
        
   for i in range(3,n,2):
        while n%i==0:
            print(i)
            n=n//i
            
primefac(36)

# To find the smallest number that evenly divides all the natural numbers from 1 to 20 
import math 
result=1
for i in range(1,21):
    result=int((result*i)/math.gcd(result,i))
print(result)

# Use the inbulit sum function to find the sum of first 100 numbers
a=[]
for i in range(1,101):
    a.append(i)
print(sum(a))

# Use teh inbuilt sum function to find the sum of squares of the first 100 numbers
a=[]
for i in range(1,101):
    result=(2*i)*(2*i)
    a.append(result)
print(sum(a))

    



    





