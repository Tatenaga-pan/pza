# pza
#learning B136

n,h,w = map(int,input().split())
sy,sx =map(int,input().split())
s = list(input())
grid = [input().split() for _ in range(h)]

for direct in s:
    if direct == 'B':
        sy += 1
    
    elif direct =='F':
        sy -= 1
        
    elif direct =='R':
        sx += 1 
    
    elif direct =='L':
        sx -= 1
        
    print(str(grid[sy-1][sx-1]))
