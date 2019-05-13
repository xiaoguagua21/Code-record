# Code-record
Here put down the code I learn or imitate
def triangles():
    L = [1]
    while True:
        yield L
        L = [1] + [L[i]+L[i+1] for i in range(len(L)-1)] + [1]


for n in triangles():
    print(n)
