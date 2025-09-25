def temperature():
    units = input("Enter the units you want to convert to (C, F): ").lower()
    match units:
        case 'c':
            print("You have chosen to convert to Celsius from Fahrenheit")
            fahrenheit = float(input("Enter your temperature in Fahrenheit: "))
            celsius = (fahrenheit - 32) * 5 / 9
            print(f"Temperature in Celsius: {celsius}")
        case 'f':
            print("You have chosen to convert to Fahrenheit from Celsius")
            celsius = float(input("Enter your temperature in Celsius: "))
            fahrenheit = (celsius * 9 / 5) + 32
            print(f"Temperature in Fahrenheit: {fahrenheit}")
        case _:
            print("Invalid unit. Please enter 'C' or 'F'.")

temperature()
