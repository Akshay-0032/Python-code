# Python-code
All basic important python programms
1. Write a program to swap two numbers.
###====with using third variable
def swap():
    ival1 = int(input("Enter the first number: "))
    ival2 = int(input("Enter the second number: "))
    ival3 = ival1
    ival1 = ival2
    ival2 = ival3
    print("After swap first number is:", ival1)
    print("After swap second number is:", ival2)

swap()

##====without using third variable
def swap():
    ival1 = int(input("Enter the first number: "))
    ival2 = int(input("Enter the second number: "))
    ival1 = ival1 + ival2
    ival2 = ival1 - ival2
    ival1 = ival1 - ival2
    print("After swap first number is:", ival1)
    print("After swap second number is:", ival2)

swap()

2. How to check number is prime or not.
def prime():
    ival = int(input("Enter the number: "))
    iCount = 0
    for i in range (1 , ival+1):
        if (ival % i == 0):
            iCount = iCount + 1
    if (iCount == 2):
        print("Entered number is prime")
    else:
        print("Entered number is not prime")

prime()

3. How to find factorial of a number 
def factorial():
    factnum = int(input("Enter the factorial number: "))
    result = 1
    for i in range (1, (factnum+1)):
        result = i * result
    print("Result of factorial number is: ",result)

factorial()
=================================================================================
def factorial():
    factnum = int(input("Enter the factorial number: "))
    i=1
    result = 1
    while (i <= factnum):
        result = i * result
        i = i + 1
    print("Result of factorial number is: ",result)

4. Print Fibonacci series.

5. How to find the sum of elements in an array?
list=[10, 20, 30, 40, 50]

def sum():
    isum = 0
    for i in list:
        isum = isum + i
    print("Sum of elements from array is: ", isum)

sum()

6. How to find maximum and minimum elements in an array? 
def maximum():
    ilist = eval(input("Enter the numbers in list: "))
    maximum = ilist[0]
    for i in ilist:
        if i > maximum:
            maximum = i
    print("Maximum value from list is:", maximum)

maximum()
=================================================================================
def minimum():
    ilist = eval(input("Enter the numbers in list: "))
    minimum = ilist[0]
    for i in ilist:
        if i < minimum:
            minimum = i
    print("Minimum value from list is:", minimum)

minimum()

7. How to find the length of the list?
ilist = [10, 20, 30, 40, 50, 60, 70, 80, 90, 100]
lenght = (len(ilist))
print("lenght of list is: ", lenght)
=================================================================================
def lenght():
    ilist = eval(input("Enter the numbers in list: "))
    lenght = 0
    for i in ilist:
        lenght = lenght + 1
    print("Lenght of list is:", lenght)

lenght()

8. How to swap first and last elements in the list
def swap():
    ilist = eval(input("Enter the numbers in list: "))
    print("First element is:",ilist[0])
    print("Last element is:",ilist[len(ilist)-1])

    Lenght   = len(ilist)
    Felement = ilist[0]
    Lelement = Felement
    Felement = ilist[Lenght-1]

    print("After swap first element is: ",Felement)
    print("After swap last element is:",Lelement)

    ilist[0] = Felement
    ilist[len(ilist)-1] = Lelement
    print("After swap list is:", ilist)

swap()

9. How to swap any two elements in the list?
def swap():
    ilist = eval(input("Enter the numbers in list: "))

    print("Before swap list is", ilist)
    Findex = int(input("Enter the first index number:"))
    Sindex = int(input("Enter the second index number:"))
    Felement = (ilist[Findex])
    Selement = (ilist[Sindex])

    temp = Felement
    Felement = Selement
    Selement = temp

    ilist[Findex] = Felement
    ilist[Sindex] = Selement
    print("After swap list is:", ilist)

swap()

10. How to remove the Nth occurrence of a given word list? 
def remove():
    ilist = eval(input("Enter the numbers in list: "))
    Number = int(input("Enter the occurrence number to be remove:"))
    print(ilist.pop(Number))
    print(ilist)

remove()

11. How to search an element in the list?
def search():
    ilist = eval(input("Enter the numbers in list: "))
    Number = int(input(("Enter an element to serach:")))
    for i in range (0, len(ilist)):
        if (Number == ilist[i]):
            print("Entered number is present in list")
            print("Index number of entered number is:", i)
            break
    else:
        print("Entered number is not present in list")

search()

12. How to clear the list?
def clear():
    ilist = eval(input("Enter the numbers in list: "))
    print("Before clear list is:", ilist)
    clear = ilist.clear()
    print("After clear list:")
    print(ilist)

clear()

13. How to reverse a list?
def reverse():
    ilist = eval(input("Enter the numbers in list: "))
    print(ilist)
    reverse = ilist.reverse()
    print(ilist)

reverse()

def reverse():
    ilist = eval(input("Enter the numbers in list: "))
    print(ilist)
    rev = ilist[::-1]
    print(rev)

reverse()

14. How to clone or copy a list?
alist = [10, 20, 30, 40, 50]
blist = (alist.copy())
print("blist is",blist)
=================================================================================
clist = [10, 20, 30, 40, 50]
dlist = clist[:]
print("dist is", dlist)

15. How to count occurrences of an element in a list?
def count():
    ilist = eval(input("Enter the numbers in list: "))
    number = int(input("Enter the value: "))
    array = {}
    for i in range(0, len(ilist)):
        if (number == ilist[i]):
            iCount = ilist.count(number)
            array[number] = iCount
    print(array)

count()

16. Find the sum of the elements in list
def sum():
    ilist = eval(input("Enter the numbers in list: "))
    sum = 0
    for i in ilist:
        sum = sum + i
    print("Sum of list is:", sum)

sum()

17. How to multiply all the numbers in the list? 
def multiplication():
    ilist = eval(input("Enter the numbers in list: "))
    number = 1
    for i in range(0, len(ilist)):
        number = number * ilist[i]
    print("multiplication of all number in list is:", number)

multiplication()

18. How to find the smallest and largest numbers on the list?
def large():
    ilist = eval(input("Enter the numbers in list: "))
    large = ilist[0]
    for i in ilist:
        if i > large:
            large = i
    print("Maximum value from list is:", large)

large()
=================================================================================
    
def small():
    ilist = eval(input("Enter the numbers in list: "))
    small = ilist[0]
    for i in ilist:
        if i < small:
            small = i
    print("Minimum value from list is:", small)

small()

19. How to find the second largest number in a list? 
ilist = eval(input("ENter the numbers in list: "))
Number = int(input("Enter the last number you want: "))
temp = ilist.sort()
Value = ilist[(len(ilist)-Number)]
print(f"The {Number} last number in list is:", Value)
=================================================================================
ilist = [10, 60, 100, 20, 90, 30, 70, 80]
large1 = ilist[0]
large2 = ilist[0]
large3 = ilist[0]
for i in range (0, len(ilist)):
    if ilist[i] > large1:
        large3 = large2
        large2 = large1
        large1 = ilist[i]
    elif ilist[i] > large2:
        large2 = ilist[i]
    elif ilist[i] > large3:
        large3 = ilist[i]
print("First large number is: ",large1)
print("Second large number is: ", large2)
print("Third large number is: ", large3)

20. How to check string is palindrome or not?
def palindrome():
    firstchar = input("Enter any string: ")
    secondchar = firstchar[-1::-1]
    if (firstchar == secondchar):
        print("Entered string is palindrome")
    else:
        print("Entered string is not palindrome")

palindrome()

21. How to reverse words in a string?
def reverse():
    char = input("Enter any word: ")
    reverse = char[::-1]
    print(f"reverse word will be like: {reverse}")

reverse()

22. How to find a substring in a string?
def substring():
    string = input("Enter the string: ")
    substr = input("Enter the substr: ")
    find = string.find(substr)
    if (find) != -1:
        print(f"Entered substr is found and index number is: {find}")
    else:
        print("Entered substr is not found")

substring()

23. How to find the length of a string?
def lenght():
    char = input("Enter any string: ")
    lenght = len(char)
    print("Lenght of enetered string is: ", lenght)

lenght()
=================================================================================

def lenght():
    char = input("Enter any string: ")
    lenght = 0
    for i in char:
        lenght = lenght+1
    print("Lenght of entered string is: ",lenght)

lenght()

24. How to check if the string contains any special character?

25. Check for URL in a string
