A=[]
m=int(input('enter no.of rows:'))
n=int(input('enter no.of columns:'))
for i in range(m):
    row=[]
    for j in range(n):
        k=int(input())
        row.append(k)
    A.append(row) 
print(A)    
B=[]
m=int(input('enter no.of rows'))
n=int(input('enter no.of columns:'))
for i in range(m):
    row=[]
    for j in range(n):
        k=int(input())
        row.append(k)
    B.append(row)
print(B)
result=[[0,0],[0,0]]
for i in range(m):
    for j in range(n):
        for k in range(n):
            result[i][j]+=A[i][k]*B[k][j]
print('resultant matrix is:')
for i in range(m):
    for j in range(n):
        print(result[i][j],end=' ')
    print()
    
    output:
    enter no.of rows:2
    enter no.of colums:2
    4
    3
    2
    1
    [[4,3],[2,1]]
    enter no.of rows:2
    enter no.of columns:2
    9
    8
    7
    6
    [[9,8],[7,6]]
    resultant matrix is:
    57 50
    25 22
