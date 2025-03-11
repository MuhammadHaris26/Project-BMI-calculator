
import streamlit as st 
import pandas as pd

st.title("BMI CALCULATOR")

height = st.slider("Enter Your Height In (cm):", 100 , 250 , 174)
weight = st.slider("Enter Your Weight In (kg):", 30 , 139 , 59)

bmi = weight / ((height/100) ** 2)

st.write(f"Your BMI is : {bmi}")

st.write("- Underweight: When BMI less than 19")
st.write("- Normal : When BMI Between 19.5 and 24.9")
st.write("- Overwieght: When BMI Between 25 and 29.9")
st.write("- Obesity: When BMI Between 30 and above")
