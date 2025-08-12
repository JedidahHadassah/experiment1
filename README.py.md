# weather-modeling
import math

# Take input from user
a = float(input("Enter a: "))
b = float(input("Enter b: "))
c = float(input("Enter c: "))

# Find the value inside square root
d = b**2 - 4*a*c

# Check the value of d (discriminant)
if d > 0:
    x1 = (-b + math.sqrt(d)) / (2*a)
    x2 = (-b - math.sqrt(d)) / (2*a)
    print("Two real roots:", x1, "and", x2)
elif d == 0:
    x = -b / (2*a)
    print("One real root:", x)
else:
    print("No real roots. The roots are complex numbers.")