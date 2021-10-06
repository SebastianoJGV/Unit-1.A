```.py
def quiz002(a, b, c):
    if abs(a-b)>abs(a-c):
        result = abs(a-b)
    elif abs(a-c) > abs(a-b):
        result = abs(a-c)
    if abs(b-c) > result:
        result = abs(b-c)
    return result
```
