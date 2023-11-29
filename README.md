# Simple Twitch Utilities
Easy and configurable utilities for Twitch!

## What's Included
- `broadcast.html`: display simple mesages on screen! Helpful if you need to go AFK or something like that.
- `timer.html`: display a timer that will count down to 00:00. Helpful for pomodoro or other tasks!

## Setup
- Download the repository as a .zip file
- Unzip and save in a convenient spot for you
- Open `config.js` in any text editor (such as Notepad)
    - `channel`: change the value within the quotes from `fletchmakes` to the name of your Twitch channel
    - `textColor`: if desired, change the value to a new color (default is an off-white)
    - `backgroundColor`: if desired, change the value to a new color (default is dark blue)

### broadcast.html
- Open OBS and create a new browser source with the following settings:
    - Local file (make sure this is checked, then click "Browse" and select the `browser.html` file)
    - Width: 1920
    - Height: 200 (you can increase this number if you plan on having long messages display)

### timer.html
- Open OBS and create a new browser source with the following settings:
    - Local file (make sure this is checked, then click "Browse" and select the `timer.html` file)
    - Width: 300
    - Height: 200

## Command Reference
The streamer and moderators can run the following commands:

### broadcast.html
    - `!bshow <message>`: displays the `<message>` that you type in on screen
    - `!bhide`: hides the message

### timer.html
    - `!tstart <number>`: starts a timer with `<number>` representing how many minutes to set the timer for. Example: `!tstart 20`
    - `!tstop`: end the timer before it finishesthe countdown
