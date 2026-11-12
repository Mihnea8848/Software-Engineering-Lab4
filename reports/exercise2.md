# Bug reports for exercise2.py

Line: 2
Problem: is_passing returns False for a grade of exactly 5, but the docstring says "5 or more".
Example: is_passing(5) returns False, expected True.
Fix: return grade >= 5

Line: 8
Problem: is_valid_password rejects passwords with exactly 8 characters, but the docstring says "at least 8 characters".
Example: is_valid_password("12345678") returns False, expected True.
Fix: return len(password) >= 8 and any(c.isdigit() for c in password)

Line: 12
Problem: clamp returns max(low, min(x, low)), which simplifies to low regardless of x, but the docstring says "x, limited to the range from low to high".
Example: clamp(10, 5, 15) returns 5, expected 10.
Fix: return max(low, min(x, high))
