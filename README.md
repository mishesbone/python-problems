# python-problems
# -*- coding: utf-8 -*-
"""
A python program to assign an (a ) or an (an) to a text entered by a user appropraitely
and print to the stdio

Created on Sun Jan 29 10:36:59 2023

@author: roboteknologies agent mishes
"""
#create a list of keys for reference
keys=["a","e","i","o","u"]
#request a text from a user
#returns an error if something other than a string literal is provided by user 
text=str(input("Enter a word:\n"))
#iterates through list items
for i in keys:
    #checks if first letter is in keys(i.e. is a vowel)
    if text[0] in keys:
        #prints the word accordingly
        print("an",text)
        #terminates the flow of the if keyword command since condition is met
        break
    #this runs where the condition if the if keyword flow of command isn't met
    else:
        #prints the text provided accordingly
        print("a",text)
        #terminates the flow of the if-else keyword command
        break
