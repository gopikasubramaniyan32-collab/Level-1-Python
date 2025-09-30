# Level-1-Python
Patterns
#Alternate rows of 1's and 0's
n=int(input())
for row in range(1,n+1):
    for col in range(1,n+1):
        print(row%2,end="")
    print()
#Box made of 1's and filled with 0's
n=int(input())
for row in range(1,n+1):
    for col in range(1,n+1):
        if(row==1 or row==n or col==1 or col==n):
            print("1",end="")
        else:
            print("0",end="")
    print()
#Print the following star Pattern
n=int(input())
for i in range(n):
    stars=n-i
    spaces=2*i
    print('*'*stars +' '*spaces+'*'*stars)
for i in range(n):
    stars=i+1
    spaces=2*(n-i-1)
    print('*'*stars +' '*spaces+'*'*stars)
#Print the Following Pattern
n=int(input())
for row in range(1,n+1):
    print("*"*row)
for row in range(n,0,-1):
    print("*"*row)
#Box filled with 1's and 0's forming a plus sign
n = int(input().strip())
mid1 = n // 2 - 1 if n % 2 == 0 else n // 2
mid2 = n // 2
for i in range(n):
    row = ""
    for j in range(n):
        if (n % 2 == 0 and (mid1 <= i <= mid2 or mid1 <= j <= mid2)) \
           or (n % 2 == 1 and (i == mid1 or j == mid1)):
            row += "0"
        else:
            row += "1"
    print(row)
#Box pattern made of center as 0 and remaining filled in 1's
n = int(input().strip())
mid1 = n//2 - 1 if n % 2 == 0 else n//2
mid2 = n//2
for i in range(n):
    row = ""
    for j in range(n):
        if mid1 <= i <= mid2 and mid1 <= j <= mid2:
            row += "0"
        else:
            row += "1"
    print(row)
#Print the pattern
n = int(input().strip())
for i in range(1, n+1):
    stars = "*" * i
    spaces = " " * (2*(n-i))
    print(stars + spaces + stars)
for i in range(n, 0, -1):
    stars = "*" * i
    spaces = " " * (2*(n-i))
    print(stars + spaces + stars)
#Plus Pattern
n = int(input().strip())
mid = n // 2  # middle index

for i in range(n):
    for j in range(n):
        if i == mid:          # middle row
            print("*", end="")
        elif j == mid:        # middle column
            print("*", end="")
        else:
            print(" ", end="")
    print()

    




    




