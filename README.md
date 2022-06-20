# Counter Strike Aimbot using Tensorflow

<p><em>GIF from this fork &darr;</em></p>

![tensorflow-counter-strike](https://user-images.githubusercontent.com/70989484/174680889-8054d1cc-764e-46b8-bed1-177d186c8c11.gif)

<p><em>GIF from the original creator &darr;</em></p>

![gif](https://user-images.githubusercontent.com/16572520/97908708-56bc5a00-1d47-11eb-9567-442237e1e7cf.gif)

<hr>

## How do I set this up on Windows?
1. Install Python 3.9.7
2. Download this repo and open up in Visual Studio Code
3. Create a virtual environment for this project <em>~ Explained Below</em>
4. Execute `pip install -r requirements.txt` in a terminal window using the venv
5. If using a GPU (<em>Only on Supported NVIDIA GPU's</em>) use <strong>CUDA 11.7</strong> (<em>don't forget to put the cuDNN dll's and zlibwapi.dll into the CUDA bin folder location</em>)
6. If using a CPU, delete the tf.device() function in aimbot.py
7. Change the name of the game window in aimbot.py if using another version of Counter Strike
8. Boot up Counter Strike and run the python file

> <strong>DON'T USE A VAC SECURED SERVER ~ YOU ARE VERY LIKELY TO GET BANNED</strong>

<hr>

## How do I use this?
* To start aimbot, hold down `t` for about a second
* To pause aimbot, hold down `y` for about a second
> Once second is about the duration of 1-2 cycles of the program. This is to make sure that the "if" statement sees that a key is pressed when it checks in that small timeframe. It isn't easy to combine HID devices and stuff like this since Tensorflow doesn't run well when using threading, and there is no parallelism in python- things can only run concurrently.
<hr>

## How to Create a Virtual Environment for Python in VS Code
### Always start with a project folder (download this repo to use as one)

Start by clicking 'New Terminal' under the  'Terminal' section on the top left part of VS Code.

Windows &darr;
- CMD  -->  `python -m venv venv`
- Powershell --> `py -m venv venv`
> **Note:** If you're using powershell, know that Microsoft makes you use `py` to reference the default installation of python. Otherwise, you will get a pop-up to the Windows Store, begging you to download their unstable version. Obviously, don't do what they're asking you to and stick with your installation.
- Do **CRTL + SHFT + P**  &rarr;  Type in 'Python: Select Interpreter' and hit enter. From there, click on the option with a star next to it. If there isn't a star next to any of them, look for .venv\Scripts\python.exe in your project folder. If there isn't a venv folder, then troubleshoot on the internet.
- Do **CTRL + SHFT + \`**  &rarr;  This should run the 'activate' file in the folder of the selected interpreter and pop-up with a terminal that says ``(venv)`` We know that the venv is working because it says '(venv)' before the project folder. From here, you can install libraries using pip without touching your main installation of python.

<hr>
