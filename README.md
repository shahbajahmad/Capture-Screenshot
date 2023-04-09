# Capture-Screenshot

This is a Python script that takes screenshots at a specified frequency and saves them to a specified directory. It uses the argparse module to parse command line arguments for the path to store the screenshot, the type of frequency (hour, minute or second), and the frequency itself. It then uses the pyautogui module to take the screenshot and the time module to wait between each screenshot.

The script first checks the type of frequency and calculates the number of seconds between each screenshot based on the frequency. If the frequency is set to a value that would result in less than 1 second between screenshots, it sets the wait time to 1 second.

It then checks if the specified directory exists and creates it if it does not.

The script then enters a while loop that continuously takes screenshots, saves them to the specified directory with a file name based on the current time, and waits for the specified number of seconds between screenshots. The loop will continue indefinitely until the user interrupts the script using the keyboard.

If the user interrupts the script, it prints a message indicating the end of the script.
