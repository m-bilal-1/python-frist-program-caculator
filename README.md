# python-frist-program-caculator
def calculator():
  print("Simple Python Calculator")
  print("Operations: + - * / ** % //")

  num1 = float(input("Enter first number: "))
  operator = input("Enter operator: ")
  num2 = float(input("Enter second number: "))

  result = None

  if operator == "+":
    result = num1 + num2
  elif operator == "-":
    result = num1 - num2
  elif operator == "*":
    result = num1 * num2
  elif operator == "/":
    if num2 != 0:
      result = num1 / num2
    else:
      print("Cannot divide by zero!")
  elif operator == "**":
    result = num1**num2
  elif operator == "%":
    if num2 != 0:
      result = num1 % num2
    else:
      print("Cannot perform modulo by zero!")
  elif operator == "//":
    if num2 != 0:
      result = num1 // num2
    else:
      print("Cannot perform floor division by zero!")
  else:
    print("Invalid operator")

  if result is not None:
    print(f"Result: {result}")


# Run the calculator
calculator()
