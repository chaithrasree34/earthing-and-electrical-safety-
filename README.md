# earthing-and-electrical-safety-
# Earthing and Electrical Safety Calculator

print("EARTHING AND ELECTRICAL SAFETY")

# Input values
voltage = float(input("Enter fault voltage (V): "))
fault_current = float(input("Enter fault current (A): "))
earth_resistance = float(input("Enter earth resistance (Ohm): "))
safety_limit = float(input("Enter maximum permitted earth resistance (Ohm): "))

# Calculate touch voltage
touch_voltage = fault_current * earth_resistance

print("\n--- RESULTS ---")
print("Earth Resistance =", round(earth_resistance, 2), "Ohm")
print("Touch Voltage =", round(touch_voltage, 2), "V")

# Check earthing condition
if earth_resistance <= safety_limit:
    print("Earthing Status: SAFE")
else:
   