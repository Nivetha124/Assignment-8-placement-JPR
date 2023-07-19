# Assignment-8-placement-JPR
# 1 Find the maximum value and its index (first occurrence) in the given array of N elements I/p : 5   12 ,55, 18 , 55, 50 O/P: 55 1
def largest(arr, n):
    # Initialize maximum element
    max = arr[0]
    for i in range(1, n):
        if arr[i] > max:
            max = arr[i]
    k=arr.index(max)
         (OR)
    k=0
    for j in arr:
        if j==max:
          print(k)
          break
        k+=1
    return max, k

arr = [10, 20, 40, 30, 40]
n = len(arr)
k=0
Ans = largest(arr, n)
print("Largest in given array ", Ans)

# 2 Find the maximum value and its index (last occurrence) in the given array of N elements
I/P
5
12 ,55, 18 , 55, 50
O/P: 55 3

# 3. From the array , count the number of elements to be added to make the sum at least X. The elements to be added should be positive even numbers only. i/P  13 N 23,28,-50,24,12,5,40,-7,-12,68,7,11,9 elements 100 X
Output: 4
Explaination:28 +24+12+40 = 104 hence 4 elements to be added to make sum up to 100

def evennumber(arr1,n,x):
    even=0
    for i in arr1:
        if i>0 and i%2==0:
            even+=i
    y=even-x
    print(y)
arr1 = [23,28,-50,24,12,5,40,-7,-12,68,7,11,9]
n = len(arr1)
x=100
evennumber(arr1, n, x)

# 4.Count the number of times the minimum value is present in the array. Display minimum value and no of times. 
I/P
6
12 ,55, 18 , 55, 50,12
O/P
12 2

def find(xlst):
    smallest = min(xlst)
    count = xlst.count(smallest)
    print(f"The smallest number is {smallest}, it occurs {count} times.")
    return smallest, count
xlst=[12 ,55, 18 , 55, 50,12]
find(xlst)


# 5. Sum the first X negative numbers in array
I/P
8
12, 34, -12, 30, -6, -8, 8, -10
3
O/P: -26

a=[]
n=int(input("enter the length of the array"))
for i in range(n):
    x=int(input("enter the next value"))
    a.append(x)
y=int(input("enter the limited value added in the list"))
sum=0
count=0
for i in a:
    if i<0:
        sum+=i
        count+=1
        if count==y:
            break
print(sum)

# 6. Print the ODD numbers in different lines but print the consecutive ODD numbers in same line.
I/P
15
10, 7 , 4 , 5 , 9 ,12 , 4 , 3, 11, 13 , 17 , 5 , 6 , 95 , 21
O/P
7
5 9
3 11 13 17 5
95 21




