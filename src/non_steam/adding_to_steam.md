# Adding Bottles to Steam
1. While in Desktop mode, open Steam by clicking on the Steam icon in your taskbar.
2. Select Library
3. Click on "ADD A GAME" in the bottom left
4. Click on the checkbox next to "Bottles" in the program list
5. Click on "ADD SELECTED PROGRAMS"

Now, when you go back to the Gaming mode, you should see the Bottles app in your library (last tab)

# Adding Bottle to Steam
**WORK IN PROGRESS**

Create a new file with a following content:
```
flatpak run com.usebottles.bottles -b BOTTLE_NAME -p PROGRAM_NAME
```

You can also specify a full path:
```
flatpak run com.usebottles.bottles -b BOTTLE_NAME -e EXE_PATH
```

# Adding Ubisoft Connect's games to Steam
**WORK IN PROGRESS**

Create a new file with a following content:
```
flatpak run com.usebottles.bottles -b BOTTLE_NAME -e EXE_PATH -a uplay://launch/APP_ID/0
```
Make sure to replace APP_ID with a game that you want to run. You can find a list of app ids [here](https://github.com/Haoose/UPLAY_GAME_ID). 