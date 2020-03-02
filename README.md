# Reynold-and-Nusselt-Calculations
Intro to Thermal Sciences Schmidt Problem 7-5

#7_5

p = 62 #lbm/ft^3
Cp = 0.998 # Btu/lbm*˚F
k = 0.3616  # Btu/hr*ft*˚F
Pr = 4.55 
m = 1.648 #lbm/ ft*hr
d = 0.0833  #ft
V = 6  #ft/s

Re = p*d*V/(m/3600)

print (f"Re = {Re}")


Nu = 0.012*((Re**0.87)-(280))*Pr**0.4

print (f"Nu = {Nu}")

Prw = 2.02

Nucorr = (((Pr/Prw)**0.11))*(Nu)

print (f"Nucorr = {Nucorr}")

h = Nucorr*k/(d)

print (f"h = {h} Btu/hr*ft^2*˚F")
