# Adding a single game to Steam
You should know how to create files and where to add them from previous chapters. The only difference now would be the .desktop file contents.

To add a single game, we should be able to just specify a direct path to an .exe file, or better, launch it via a launcher.

## Ubisoft Connect
```properties
[Desktop Entry]
Name=A Game
Comment=Pew pew
Exec=flatpak run --command=bottles-cli com.usebottles.bottles run -b BOTTLE_NAME -p "Ubisoft Connect" -a uplay://launch/APP_ID/0
Icon=input-gaming
Terminal=false
Type=Application
Categories=Game;
```

Make sure to replace APP_ID with a game that you want to run. You can find a list of app ids [here](https://github.com/Haoose/UPLAY_GAME_ID). 