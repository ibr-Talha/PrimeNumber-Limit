# PrimeNumber-Limit
Print the prime numbers which are between 1 to entered limit number (n).

liste = []
x = int(input(" "))

for n in range (1, x):
    count = 0
    t = n//2
    for i in range(2, (t + 1)):
        if(n % i == 0):
            count = count + 1
            break
 
    if (count == 0 and n > 1):
      liste.append(n)

print(liste, end = '  ')
