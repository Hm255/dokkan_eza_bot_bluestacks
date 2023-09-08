# Dokkan Battle EZA Farming Bot

![Dokkan Battle Auto-Play Script](https://github.com/feijoes/dokkan_eza_bot/assets/74252371/c2f5c2bf-1e0c-4ebe-8792-ec55113311ce)

## Introduction

The Dokkan Battle EZA Farming Bot is a Python script designed to automate the process of farming the Extreme Z-Awakening levels in Dragon Ball Z Dokkan Battle. The script runs on your computer and interacts with the game on your phone or your computer if you are using bluestacks.

_This bot is no a autoclicker_; it not only completes the levels but also manages the current level of the EZA and switches between different EZAs.


If you encounter any errors or have any doubts, you can create an issue or contact me at pcaladomoura@gmail.com.

## Features

- Automated farming of Extreme Z-Awakening levels in Dokkan Battle.
- It identifies buttons and actions using images, so it can adapt to different screen sizes and resolutions.
- Can swipe between eza and only

## Requirements

1. You need an Android device with USB debugging enabled. This allows the script to communicate with the phone via a USB cable.
2. Get you phone in [developers options](https://www.digitaltrends.com/mobile/how-to-get-developer-options-on-android/) and enable the options:
      * **Don't lock screen**: This prevents the screen from locking to ensure uninterrupted gameplay.
      * **USB Debugging**

3. Your computer should have Python 3.x installed. You can download it from the [official Python website](https://www.python.org/downloads/).
4. Install [tesseract](https://linuxhint.com/install-tesseract-windows/) in your computer

## Bluestacks setup

**The first 2 steps for using this bot on phone can be ignored for the bluestacks setup. Steps 2-5 only need to be done once**

1. Enter the advanced section in bluestacks settings and enable adb bridging. 
   
   When using bluestacks 5, under that option should be a message (english: 'connect to Android at [insert localhost here]'). The last 5 numbers will be different every time you run bluestacks and will be your `session number`.

2. find the phone section in bluestacks settings and select a phone you want to simulate.
3. [Go here](https://www.gsmarena.com/compare.php3). Find the display resolution of the phone you selected in bluestacks (quality and DPI/PPI), then enter them as custom selections into the display section of bluestacks settings to properly simulate your phones quality, this will help the bot find buttons.

4. Enter bluestacks game controls settings and turn off the on-screen controls to not distract the bot

5. Download the zip that applies to your computer(OS) for adb [from this link](https://www.xda-developers.com/install-adb-windows-macos-linux/). Scroll down to find non-phone instructions and follow those instructions until you are inside the file path /platform-tools/ (restart your terminal before the next step). 

6. In /platform-tools/ type in `adb connect localhost:your session number`, 'connected to localhost:your session number' should appear. Check using `adb devices` to check if your device is connected.

7. Your computer should have Python 3.x installed. You can download it from the [official Python website](https://www.python.org/downloads/).
8. Install [tesseract](https://linuxhint.com/install-tesseract-windows/) in your computer

## Usage 

### All EZAs (level 31)

1. Launch the Dokkan Battle app on your Android device and go to eza section
2. Scroll down to the bottom of the EZA events, as the bot will change EZA events by swiping upwards.
3. Open a terminal or command prompt in the project directory.
4. install the requirements
  ```py
  pip install -r requirements.txt
  ```
  And run 
  ```
  python main.py
  ```
### Infinite Mode
1. Launch the Dokkan Battle app on your Android device and go to eza section
2. Select the EZA you want to farm infinitely
3. Open a terminal or command prompt in the project directory.
4. install the requirements
  ```py
  pip install -r requirements.txt
  ```
  And run 
  ```
  python main.py inf
  ```
## Disclaimer

This project is intended for educational and personal use only. The use of automation bots in games may violate the game's terms of service, and using this script may carry the risk of account suspension or banning. The developer of this project is not responsible for any consequences resulting from the use of this bot.


## Contributing

Contributions to this project are welcome! If you encounter any issues, have suggestions for improvements, or want to add new features, feel free to open an issue or submit a pull request.

## License

This project is licensed under the [MIT License](LICENSE).

---

Feel free to modify the README according to your project's specific details, and don't forget to add a proper license file (e.g., `LICENSE`) to your project if you plan to share it with others.
