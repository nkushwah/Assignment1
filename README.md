#!/usr/bin/env python
# coding: utf-8

# ## TASK 1

# ###  Install Jupyter notebook and run the first program and share the screenshot of the output.

# In[4]:


print('Hello world!!')


# 
# 

# ### Write a program which will find all such numbers which are divisible by 7 but are not a multiple of 5, between 2000 and 3200 (both included). The numbers obtained should be printed in a comma-separated sequence on a single line.

# In[17]:


result = []
for item in range(2000,3201):
    if(item%7==0 and item%5!=0):
        result.append(item)
print(', '.join([str(x) for x in result]))


# 
# 

# ### Write a Python program to accept the user's first and last name and then getting them printed in the the reverse order with a space between first name and last name.

# In[26]:


if __name__ == '__main__':
    FirstName = input()
    LastName = input()
    print(f"{LastName} {FirstName}")


# 
# 

# ### Write a Python program to find the volume of a sphere with diameter 12 cm. Formula: V=4/3 * π * r 3

# In[32]:


import math 
dia = 12 
volume = round(((4/3)*(math.pi)*(dia**3)),2)
print(volume)
print(f"Volume of {dia}cm of sphere is {volume}cubic cm")


# 
# 

# ## Task 2:

# ### Write a program which accepts a sequence of comma-separated numbers from console and generate a list.

# In[40]:


if __name__ == '__main__':
    stringInput = input()
    listInput = stringInput.split(',')
    print(listInput)


# 
# 

# ### Create the below pattern using nested for loop in Python.
# *
# * *
# * * *
# * * * *
# * * * * *
# * * * *
# * * *
# * *
# *

# In[65]:


n = 10
for item in range(1,n):
    if item<=5:
        for loop1 in range(0,item):
            print(f"* ", end=" ")
        print("\n")
    else:
        for loop2 in range(0,n-item):
            print(f"* ", end=" ")
        print("\n")


# 
# 

# ### Write a Python program to reverse a word after accepting the input from the user.
# Sample Output:
# Input word: AcadGild
# Output: dilGdacA

# In[68]:


if __name__ == '__main__':
    string = input()
    print(string[::-1])


# 
# 

# ### Write a Python Program to print the given string in the format specified in the sample output.
# WE, THE PEOPLE OF INDIA, having solemnly resolved to constitute India into a
# SOVEREIGN, SOCIALIST, SECULAR, DEMOCRATIC REPUBLIC and to secure to all
# its citizens
# Sample Output:
# WE, THE PEOPLE OF INDIA,
# having solemnly resolved to constitute India into a SOVEREIGN, !
# SOCIALIST, SECULAR, DEMOCRATIC REPUBLIC
# and to secure to all its citizens

# In[71]:


print(f"WE, THE PEOPLE OF INDIA,\nhaving solemnly resolved to constitute India into a SOVEREIGN, !\nSOCIALIST, SECULAR, DEMOCRATIC REPUBLIC\nand to secure to all its citizens")

