
Navigation Menu

Code
Issues
Pull requests
BreadcrumbsPython_Diary_App_withGUI
/README.md
Latest commit
GeorgeDavila
GeorgeDavila
5 years ago
History
85 lines (60 loc) · 4.46 KB
File metadata and controls

Preview

Code

Blame
Python Diary App using tkinter GUI
A python diary desktop application

A fun diary application written in python using the tkinter GUI module. Meant to be as simple as possible to show how easy it is to create python desktop apps that might more often be made in JS. Only some basic python knowledge is required.

Of course one could easily merge everything into one script but the purpose of this project is to show how we can create a flexible and modular GUI in python.

We make a diary for a change of pace from the more common numerical application one might see in python

Diary GUI and desktop shortcut:

Alt Text

Diary GUI used to make a diary entry and look at the diary:

Alt Text

Dependencies
python 3
pyinstaller
Only if you want to make/modify your own app instead of running mine
tkinter
Should be installed with python, can just run 'pip install tkinter' otherwise
Running
Run App
Just click the app (tk_diarygui.exe) to run it
Alternatively, go to file directory and type 'start tk_diarygui.exe
Build the App on your device:
Navigate to directory containing the python scripts and enter the following commandto create an executable application: pyinstaller -w -F -i book_icon.ico tk_diarygui.py

Drag the executable out of the dist directory and into your main diary_app directory
You can now run your .exe app from terminal or clicking on it
You can even make a desktop shortcut and run it from there!
-w stops the command terminal from opening when we run the desktop app -F wraps the dist up into the one simple .exe file -i assigns the book_icon.ico image as the app's desktop icon (need to do this with an ico file, can find or convert imgs to this online)

Run Main Python Codes
python tk_diarygui.py
initializes the GUI, can run the write2diary.py file just by writing in the text and clicking the blue 'write' button
python write2diary.py --input my_text_use_underscores_for_whitespaces
Don't need to run this, as mentioned above.
More annoying to use this, as we need to use underscores for spaces. Whereas in GUI we can just rite normally in the textbox
Run Misc Python Codes
python strrep_example.py --input my_text_use_underscores_for_whitespaces
Just an example of the process we use to change underscores from the input into whitespaces
Do it this way to try and minimize the amount of code without having to input any text into anything other than the GUI, the whole point is to interact with a GUI not the terminal
python write2diary.py --input my_text_use_underscores_for_whitespaces
Lesser version of write2diary.py, this version excludes the automatic writing of the date/time
