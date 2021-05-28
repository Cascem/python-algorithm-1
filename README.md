# python-algorithm-1
pinary number algorithm
import sys

def f(n):
    if n==1 or n==2:
        return 1
    x=1
    y=1
    for i in range(n-2):
        z=x+y
        x=y
        y=z
    return y

k = f(int(sys.stdin.readline()))
print(k)
