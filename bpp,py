# simple_calculator.py

import streamlit as st

# Title for the web app
st.title("Simple Calculator")

# Input fields
num1 = st.number_input("Enter first number", value=0.0)
num2 = st.number_input("Enter second number", value=0.0)

# Dropdown menu to select operation
operation = st.selectbox("Select operation", ("Addition", "Subtraction", "Multiplication", "Division"))

# Perform the selected operation
result = None
if operation == "Addition":
    result = num1 + num2
elif operation == "Subtraction":
    result = num1 - num2
elif operation == "Multiplication":
    result = num1 * num2
elif operation == "Division":
    if num2 != 0:
        result = num1 / num2
    else:
        st.error("Division by zero is not allowed!")

# Display result
if result is not None:
    st.success(f"The result of {operation.lower()} is: {result}")
