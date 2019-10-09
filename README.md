# Mobile-3.0-iOS-Тестовое задание №2 - Python 3
N = int(input())
a = [int(i) for i in input().split()]
a.sort()
i = 0
while a[i]%3 != 0:
    i += 1
j = 0
while i < len(a):
    a.insert(j, a[i])
    del a[i+1]
    i += 3
    j += 1
print(a)
