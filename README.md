# temperature-conversion
def CelsiusToFahrenheit(c):
    return (c*9/5)+32
def CelsiusToKelvin(c):
    return c+273.15
def FahrenheitToCelsius(f):
    return (f-32)*5/9
def FahrenheitToKelvin(f):
    return (f-32)*5/9+273.15
def KelvinToCelsius(k):
    return k-273.15
def KelvinToFahrenheit(k):
    return (k-273.15)*9/5+32

temperature =float(input("Enter Temperature value: "))
unit=input("Enter Temperature unit(C for celsius,F for fahrenheit,K for Kelvin): ")

if(unit=="C"):
    print("Temperature in Farenheit:",CelsiusToFahrenheit(temperature))
    print("Temperature in Kelvin:",CelsiusToKelvin(temperature))
elif(unit=="F"):
    print("Temperature in Celsius:",FahrenheitToCelsius(temperature))
    print("Temperature in Kelvin:",FahrenheitToKelvin(temperature))
elif(unit=="K"):
    print("Temperature in Celsius:",KelvinToCelsius(temperature))
    print("Temperature in Fahrenhiet:",KelvinToFahrenheit(temperature))
else:
    print("Invalid Temperature unit")