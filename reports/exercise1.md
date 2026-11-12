# Bug reports for exercise1.py

Line: 3
Problem: is_even returns True for odd numbers (e.g., 1, 3, 5) because it checks n % 2 == 1, but the docstring says it should be true for even numbers. The correct condition for even numbers is n % 2 == 0.
Example: is_even(2) returns False, expected True.
Fix: return n % 2 == 0

Line: 8
Problem: rectangle_area returns the sum of width and height, but the docstring says it should return the area of a rectangle, which is width times height.
Example: rectangle_area(4, 5) returns 9, expected 20.
Fix: return width * height

Line: 13
Problem: double returns n + 2, but the docstring says it should return twice the number n, i.e., n * 2.
Example: double(5) returns 7, expected 10.
Fix: return n * 2
