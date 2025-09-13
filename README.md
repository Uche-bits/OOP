# OOP
class Rectangle:
    def __init__(self, length, width):
        self.length = length
        self.width = width

    def calculate_area(self):
        return self.length * self.width

    def calculate_perimeter(self):
        return 2 * (self.length + self.width)

    def is_square(self):
        return self.length == self.width

# Example Usage

# Creating a rectangle object
my_rectangle = Rectangle(length=10, width=5)

# Creating a square object
my_square = Rectangle(length=7, width=7)

# Using the methods for the first rectangle
print(f"Rectangle with length = {my_rectangle.length} and width = {my_rectangle.width}")
print(f"Area: {my_rectangle.calculate_area()}")
print(f"Perimeter: {my_rectangle.calculate_perimeter()}")
print(f"Is it a square? {my_rectangle.is_square()}")
print("-" * 20)

# Using the methods for the square
print(f"Rectangle with length = {my_square.length} and width = {my_square.width}")
print(f"Area: {my_square.calculate_area()}")
print(f"Perimeter: {my_square.calculate_perimeter()}")
print(f"Is it a square? {my_square.is_square()}")

