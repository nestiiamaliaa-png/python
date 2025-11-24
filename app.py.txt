import streamlit as st

st.title("Program Mengurutkan Tiga Bilangan")

a = st.number_input("Masukkan bilangan pertama:", value=0)
b = st.number_input("Masukkan bilangan kedua:", value=0)
c = st.number_input("Masukkan bilangan ketiga:", value=0)

if st.button("Urutkan"):
    angka = [a, b, c]
    angka.sort()
    st.success(f"Urutan bilangan dari yang paling kecil: {angka[0]}, {angka[1]}, {angka[2]}")
