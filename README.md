# Kadane-s-Algorithm
def max_function(arr):
    current_max=arr[0]
    get_max=arr[0]
    for i in range(1,len(arr)):
        current_max=max(arr[i],current_max+arr[i])
        get_max=max(current_max,get_max)
        #current_max=current_max+arr[i]
        #if current_max<0:
        #    current_max=0
        #if get_max<current_max:
        #    get_max=current_max
    return get_max    
test_case=int(input())
for i in range(test_case):
    size_arr=int(input())
    arr=list(map(int,input().split()))
    print(max_function(arr))





  
