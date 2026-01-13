# quadratic-equation-solver-69-100

import math

a = float(input())
b = float(input())
c = float(input())

if a != 0.0:
    d = b**2 - 4*a*c

    if d == 0.0:
        r = -b / (2*a)
        print(r, r)
    elif d > 0.0:
        r1 = (-b + math.sqrt(d)) / (2*a)
        r2 = (-b - math.sqrt(d)) / (2*a)
        print(r1, r2)
    else:
        rp = -b / (2*a)
        ip = math.sqrt(-d) / (2*a)
        print(f"{rp} + i{ip}", f"{rp} - i{ip}")
else:
    print("Not a quadratic equation")
