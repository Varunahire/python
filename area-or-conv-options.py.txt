# -*- coding: utf-8 -*-
"""
Created on Wed Apr 24 09:50:51 2024

@author: mevic
"""
import area_funct as area
import conversion_funct as conv

print("Press 1 to calculate Area")
print("Press 2 to calculate Conversion")
choice=int(input("Enter the choice : "))
if choice==1:
    print("select areas from below to calculate")
    print("Press 1 for area of circle")
    print("Press 2 for area of square")
    print("Press 3 for area of rectangle")
    print("Press 4 for area of triangle")
    
    choose_area=int(input("Enter the option given above to calculate area : "))
    
    if choose_area==1:
        num=int(input("enter the radius : "))
        area.areacircle(num)
    
    elif choose_area==2:
        num=int(input("enter the number for square : "))
        area.areasquare(num)
        
    elif choose_area==3:
        length=int(input("enter the length : "))
        breath=int(input("enter the breath : "))
        area.arearectangle(length,breath)
        
    elif choose_area==4:
        base=int(input("enter the base : "))
        height=int(input("enter the height : "))
        area.areatriangle(base, height)
    else:
        print("invalid option")
        
elif choice==2:
    print("select conversion from below to calculate")
    print("Press 1 for cm to meter")
    print("Press 2 for inch to cm")
    print("Press 3 for area of fahrenheit to celsius")
    choose_conv=int(input("Enter the option given above for coversion : "))
    
    if choose_conv==1:
        cm=int(input("enter the cm "))
        conv.cm_to_meter(cm)
    
    elif choose_conv==2:
        inch=int(input("enter the inch "))
        conv.inch_to_cm(inch)
        
    elif choose_conv==3:
        far=int(input("enter the fahrenheit "))
        conv.far_to_cel(far)
    else:
        print("invalid option")
        
else:
    print("option does not exist , select from the given options")

