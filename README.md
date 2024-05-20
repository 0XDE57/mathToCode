# math to code
some examples of converting math equations to code. 

todo: fix mathjax
```math
y = \sum_{n=100}f(n)
```

```python
# f() is not defined in above equation so just squaring in this example
def f(n):
    return n * n

# y = sum(f(n)) where n = [0 to 100]
y = 0
for n in range(101):
    fn = f(n)
    y += fn
    print(str(n) + ": " + str(fn))

print("y = " + str(y))
```
note 101 which is n+1 due to 0 based indexing in range() 

output n: f(n) and y
```
0: 0
1: 1
2: 4
3: 9
4: 16
5: 25
6: 36
7: 49
8: 64
9: 81
10: 100
11: 121
12: 144
13: 169
...
96: 9216
97: 9409
98: 9604
99: 9801
100: 10000
y = 338350
```

---
I was gonna do a bunch more but I am lazy and can't seem to focus. Anywho, check this out:

https://www.youtube.com/watch?v=ba3dYob18_A
