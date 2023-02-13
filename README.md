# Using_class_functions
using class functions in python programming language
#Task 1
#income of the employee
n=int(input("enter the working hours:"))
working_hourse=n*250
p=int(input("enter the extra working hours:"))
extra_time=p*350
monthly_income=working_hourse+extra_time
print(monthly_income,"monthly income")
annual_income=12*monthly_income
print(annual_income,"annual income")

#Task 2
#Electricity bill
type=(input("Connection type:"))
if (type == "Household"):
  units=float(input("Enter the no. units of electricity consumed:"))
  if units <= 100:
    bill=units*0.50
  elif units>=101 and units<=200:
    bill = 50 + ((units-100) * 0.75)
  elif units>=201 and units<=300:
    bill= 50+75 +((units-200) * 1.20)
  else:
    bill= 50+75+120 +((units-300) * 1.50)
elif (type == "Commercial"):
  units=float(input("Enter the no. units of electricity consumed:")) 
  if units <= 100:
    bill=units*1
  elif units>=101 and units<=200:
    bill = 100 + ((units-100) * 1.5)
  elif units>=201 and units<=300:
    bill= 100+150 +((units-200) * 2.4)
  else:
    bill= 100+150+240 +((units-300) * 3)
else:
  print("select correct type")

print("Total bill amount",bill)

#electricity bill
type=(input("Connection type:"))
units=float(input("Enter the no. units of electricity consumed:"))
#for Household
while (type == "Household"):
  if units <= 100:
    bill=units*0.50
    break
  elif units>=101 and units<=200:
    bill = 50 + ((units-100) * 0.75)
    break
  elif units>=201 and units<=300:
    bill= 50+75 +((units-200) * 1.20)
    break
  elif units>=301:
    bill= 50+75+120+((units-300) * 1.50)
    break
#for Commercial 
while (type == "Commercial"):
    if (units <= 100):
      bill=units*1
      break
    elif (units>=101 and units<=200):
      bill = 100 + ((units-100) * 1.5)
      break
    elif (units>=201 and units<=300):
      bill= 100+150 +((units-200) * 2.4)
      break
    else:
      bill= 100+150+240 +((units-300) * 3)
      break
print("Total bill amount",bill)
