```.py
def perfectN(n):
    '''
    @param n: input to be factored 
    '''
    factor = [] 
    isSum = "FALSE"
    #For loop can not start at 0 due to 0%0
    for num in range(1,n-1):
        if n%num == 0:
            factor.append(num)
    if sum(factor) == n:
        isSum = "TRUE"
    return factor, isSum

x = perfectN(10)
print(x)
