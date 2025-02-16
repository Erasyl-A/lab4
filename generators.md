# 1
def square_generator(N):
    """Generator that yields squares of numbers from 0 to N."""
    for i in range(N + 1):
        yield i ** 2

# Example usage
if __name__ == "__main__":
    N = 10
    for square in square_generator(N):
        print(square)
# 2
def even_numbers_generator(n):
    for i in range(0, n + 1, 2):
        yield i

if __name__ == "__main__":
    n = int(input("Enter a number: "))
    print(", ".join(map(str, even_numbers_generator(n))))
# 3
def divisible_by_3_and_4(n):
    for i in range(n + 1):
        if i % 3 == 0 and i % 4 == 0:
            yield i

if __name__ == "__main__":
    n = int(input("Enter a number: "))
    print("Numbers divisible by 3 and 4:", list(divisible_by_3_and_4(n)))
# 4
def squares(a, b):
    for i in range(a, b + 1):
        yield i ** 2

if __name__ == "__main__":
    a = int(input("Enter the start number (a): "))
    b = int(input("Enter the end number (b): "))
    
  print("Squares from", a, "to", b, ":")
    for square in squares(a, b):
        print(square)
  # 5
  def countdown(n):
    for i in range(n, -1, -1):
        yield i

if __name__ == "__main__":
    n = int(input("Enter a number: "))
    print("Countdown from", n, "to 0:")
    for num in countdown(n):
        print(num)
