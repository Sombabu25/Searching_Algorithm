# Searching_Algorithm

# ------Binary_search----------

def binary_search(arr,target):
    l=0
    r=len(arr)-1
    while l<=r:
        mid=(l+r)//2
        
        if arr[mid]==target:
            return mid
            
        elif arr[mid]<target:
            l = mid+1
        
         
        else:
            r = mid-1
            
    return False

lst=[10,11,12,14,16,25,29,32,35]

result=binary_search(lst,32)
print(result)
    
