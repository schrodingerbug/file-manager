import os #This library is for Windows
import subprocess #This library is for Mac and Linux(any version)
import platform #This is to check what the hell you are even using

filename = input("Please enter your file name: ")

#Note:This is in the README as well,but to type files in,you do it like this:
#If your file is in the same folder as this program file,just type it with its type.For example 'file.txt'.
#Elif your file is in another folder,you have to type that in.For example 'C:\blah\blah\blah\blah\file.txt'.To get this file directory name,I would recommend using a terminal.Well,unless you are either a masochist or remember it.
#Also,you have to have a main app for every file type.What I mean is,you need to set a main app to open files for every file type.For example,for .txt,the app is Notepad.

try:
    if platform.system() == "Windows":#For the average Joe
        os.startfile(filename)
    elif platform.system() == "Darwin":  #For the Apple guys(rich bastards...I mean,1000 bucks for a laptop?Jesus.)
        subprocess.run(["open", filename])
    else:  # For the Linux bros...or whatever else you may have.Is there even an operating system besides these 3?Eh,whatever.
        subprocess.run(["xdg-open", filename])
except FileNotFoundError:
    print("Invalid file name.")

#I have put a test.txt file in the repo,try testing that out with the program(Spoiler Alert:It works!)