
#User function Template for python3

def game_with_number (arr, n) : 
    a = []
    # b = []
    for i in range(0,n-1):
        xor = arr[i] ^ arr[i+1]
        a.append(xor)
    c = arr[-1]
    a.append(c)
    
    return a
    #Complete the function

#{ 
#  Driver Code Starts
#Initial Template for Python 3


for _ in range(0,int(input())):
    
    n = int(input())
    arr = list(map(int,input().strip().split()))
    res = game_with_number(arr, n);
    print(*res)




# } Driver Code Ends
