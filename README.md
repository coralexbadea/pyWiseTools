﻿# pyWiseTools
 pip install pyWiseTools
# Example
```
from pyWiseTools.pyWiseTools import *
           
while True:
    # Capture the screen
    screenshot_gray = capture_screen(gray=True)
    matched_coord = get_word_coordinates(screenshot_gray, 'robot')

    if matched_coord:
        print("matched")
        click_dotted_line_x((matched_coord[0],matched_coord[1]), range(-10,-300,-10))
    time.sleep(1) 
```
