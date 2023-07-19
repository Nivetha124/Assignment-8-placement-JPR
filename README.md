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



