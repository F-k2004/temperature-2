# temperature_converte.py

def celsius_to_fahrenheit(c):
    return (c * 9/5) + 32

def fahrenheit_to_celsius(f):
    return (f - 32) * 5/9

def celsius_to_kelvin(c):
    return c + 273.15

def kelvin_to_celsius(k):
    return k - 273.15

def main():
    print("🌡️ مبدل دما (Celsius ↔ Fahrenheit ↔ Kelvin) 🌡️")

    while True:
        print("\nانتخاب کنید:")
        print("1. سلسیوس ➡️ فارنهایت")
        print("2. فارنهایت ➡️ سلسیوس")
        print("3. سلسیوس ➡️ کلوین")
        print("4. کلوین ➡️ سلسیوس")
        print("5. خروج")

        choice = input("گزینه: ")

        if choice == "1":
            c = float(input("دما به سلسیوس: "))
            print(f"✅ {c}°C = {celsius_to_fahrenheit(c):.2f}°F")
        elif choice == "2":
            f = float(input("دما به فارنهایت: "))
            print(f"✅ {f}°F = {fahrenheit_to_celsius(f):.2f}°C")
        elif choice == "3":
            c = float(input("دما به سلسیوس: "))
            print(f"✅ {c}°C = {celsius_to_kelvin(c):.2f}K")
        elif choice == "4":
            k = float(input("دما به کلوین: "))
            print(f"✅ {k}K = {kelvin_to_celsius(k):.2f}°C")
        elif choice == "5":
            print("👋 خداحافظ!")
            break
        else:
            print("❌ گزینه نامعتبر!")

if __name__ == "__main__":
    main()
