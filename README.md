# math to code
some examples of converting math equations to code

todo: fix mathjax
```math
y = \sum_{n=100}f(n)
```

```python
# f() is not defined in above equation so just squaring in this example
def f(n):
    return n * n


# y = sum(f(n)) where n = [0 to 100]
total_sum = 0
for n in range(100):
    y = f(n)
    total_sum += y
    print(str(n) + ": " + str(y))

print("sum: " + str(total_sum))
```

output n: f(n) and sum
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
sum: 338350
```

