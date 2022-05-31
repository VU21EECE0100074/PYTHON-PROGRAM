# PYTHON-PROGRAM
1.Write a program to read 10 numbers from a files.Write the even numbers and odd numbers to seperate files even.txt and odd.txt
*Note: Before executing the code,create a even_odd.txt and enter a n numbers in it*

file = open("even_odd.txt","rt") 
for i in file: 
    if i.strip: 
        num = int(i) 
        if (num % 2 == 0): 
            even = open("even.txt","a") 
            even.write(str(num)) 
            even.write("\n") 
        else: 
            odd = open("odd.txt","a") 
            odd.write(str(num)) 
            odd.write("\n")
             
Output:
      *Two new .txt files are created ie,even.txt and odd.txt*
*even.txt:
2
4
6
8

*odd.txt:
1
3
5
