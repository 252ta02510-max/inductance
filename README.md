import math

# Inputs
N = int(input("Enter number of turns: "))
A = float(input("Enter cross-sectional area (m^2): "))
l = float(input("Enter length of coil (m): "))
mu_r = float(input("Enter relative permeability: "))

# Permeability of free space
mu_0 = 4 * math.pi * 10**-7

# Calculate inductance
L = (mu_0 * mu_r * N**2 * A) / l

print("Inductance of the coil =", L, "H")