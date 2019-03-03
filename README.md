# Assignment3_python_Numpy1

##Write a function to compute 5/0 and use try/except to catch the exceptions.



In [1]:


def throws():
    return 5/0



In [5]:


try:
    throws()
except ZeroDivisionError:
    print("division by zero!")
except (Exception, err):
    print('Caught an exception')
finally:
    print ('In finally block for cleanup')



division by zero!
In finally block for cleanup
In [ ]:


​



In [ ]:


## #Implement a Python program to generate all sentences where subject is in
#["Americans", "Indians"] and verb is in ["Play", "watch"] and the object is in
#["Baseball","cricket"].



In [6]:


subject=["Americans","Indians"]
verbs=["play","watch"]
objects=["Baseball","Cricket"]
​
# Using nested looping to produce the expected result/output
for i in subject:
    for j in verbs:
        for k in objects:
            print(i+" "+j+" "+k+".")



Americans play Baseball.
Americans play Cricket.
Americans watch Baseball.
Americans watch Cricket.
Indians play Baseball.
Indians play Cricket.
Indians watch Baseball.
Indians watch Cricket.
