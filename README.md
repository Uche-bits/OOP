# OOP
class Rectangle:
    """
    A class to represent a rectangle.

    Attributes:
        length (float or int): The length of the rectangle.
        width (float or int): The width of the rectangle.
    """

    def __init__(self, length, width):
        """
        The constructor for the Rectangle class.

        Args:
            length (float or int): The length of the rectangle.
            width (float or int): The width of the rectangle.
        """
        # We use 'self.attribute' to store the values for the specific object
        self.length = length
        self.width = width

    def calculate_area(self):
        """
        Calculates the area of the rectangle.

        Returns:
            float or int: The area of the rectangle (length * width).
        """
        return self.length * self.width

    def calculate_perimeter(self):
        """
        Calculates the perimeter of the rectangle.

        Returns:
            float or int: The perimeter of the rectangle (2 * (length + width)).
        """
        return 2 * (self.length + self.width)

    def is_square(self):
        """
        Checks if the rectangle is also a square.

        A square is a rectangle where all sides are equal.

        Returns:
            bool: True if the length is equal to the width, False otherwise.
        """
        return self.length == self.width

# --- Example Usage ---

# Creating a rectangle object
my_rectangle = Rectangle(length=10, width=5)

# Creating a square object (which is also a type of rectangle)
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

