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
