# randompasswordgenerator
import random
import string

print("Welcome to the Passoword Generator!")

a = int(input("How many letters would you like?\n"))
b = int(input("How many numbers would you like?\n"))
c = int(input("How many symbols would you like?\n"))
l1 = []
l = string.ascii_letters
n = string.digits
p = string.punctuation

for i in range(a):
    i=random.choice(l)
    l1.append(i)

for i in range(b):
    i=random.choice(n)
    l1.append(i)

for i in range(c):
    i=random.choice(p)
    l1.append(i)
print("Before your password:",l1)
random.shuffle(l1)
print("After your password:",l1)
print("Your password is:","".join(l1))
