<img src="icon.png" alt="Icon" width="128">

NUS Exam Paper Downloader
===============

Simple script to download exam papers from the NUS database. Requires NUSNET login.

Runs on Python 3.9 now!

### Releases
Along the sidebar, you can download the latest version for macos. 

Right click on the .app file and click "show package contents". Go to the "MacOS" folder and open a terminal in that folder and type the following to give it permissions to run.

```
chmod +x "NUS Exams Paper Downloader"
```

Note: You have to right click to open for first open

On another Note:
- However, currently as of 13 April, 16:44, it seems that the database for past year papers is facing some issues with verification. Yet, after throwing incorrect authentication errors back at the user, the user is actually already signed in. Currently, this can be bypassed by simply removing the return statement in the if_else clause in examdownloader.py. To do that, you will have to build the application for yourself for now.

### Using via Command Line
```
$ python examdownloader-cli.py
```

The required username and target destination can be set in the script or passed as a command line argument.
If no command line arguments are provided, the user is prompted for input.

### Using via a Graphical User Interface
```
$ python examdownloader-gui.py
```


### Compiling the Binary

1. Install `pyinstaller`:
  ```
  $ pip install pyinstaller
  ```

2. Compile the app:
  ```
  $ pyinstaller build.spec
  ```
The compiled app can be found inside the `dist` folder.

### Credits

- Oh Shunhao [(https://github.com/Ohohcakester)](https://github.com/Ohohcakester)
- Liu Xinan [(https://github.com/xinan)](https://github.com/xinan)
- Yangshun Tay [(https://github.com/yangshun)](https://github.com/yangshun)
