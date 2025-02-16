# 1
import math

def degree_to_radian(degree):
    return degree * (math.pi / 180)

if __name__ == "__main__":
    degree = float(input("Enter degree: "))
    print("Radian:", round(degree_to_radian(degree), 6))
# 2
import math

def degree_to_radian(degree):
    return degree * (math.pi / 180)

def trapezoid_area(height, base1, base2):
    return (base1 + base2) * height / 2

if __name__ == "__main__":
    degree = float(input("Enter degree: "))
    print("Radian:", round(degree_to_radian(degree), 6))
    
  height = float(input("Enter height: "))
    base1 = float(input("Enter first base: "))
    base2 = float(input("Enter second base: "))
    print("Trapezoid Area:", trapezoid_area(height, base1, base2))
# 3
import math

def regular_polygon_area(sides, length):
    return (sides * (length ** 2)) / (4 * math.tan(math.pi / sides))

# Example usage
if __name__ == "__main__":
    sides = int(input("Enter number of sides: "))
    length = float(input("Enter length of a side: "))
    print("The area of the polygon is:", regular_polygon_area(sides, length))
# 4
import math

def regular_polygon_area(sides, length):
    return (sides * (length ** 2)) / (4 * math.tan(math.pi / sides))

def parallelogram_area(base, height):
    return base * height

if __name__ == "__main__":
    sides = int(input("Enter number of sides: "))
    length = float(input("Enter length of a side: "))
    print("The area of the polygon is:", regular_polygon_area(sides, length))
    
  base = float(input("Enter length of base: "))
    height = float(input("Enter height of parallelogram: "))
    print("The area of the parallelogram is:", parallelogram_area(base, height))
