# Highlighted Message

This is a Streamer.Bot automation that will display a highlighted message on
your stream via a Browser source.

## Installation

1. Download this repository
2. In OBS, Create a new Scene named `[TPL] Highlighted Message`. Within that
   Scene, create a new Browser source named `Highlighted Message`, and point it
   to `highlighted-message.html`. I used a width of 1080 and a height of 600.
3. Import the contents of `highlighted-message.streamerbot.txt` into
   Streamer.Bot.
4. In the action `Manually Highlight Message`, change the first action (setting
   the output path) to the path that this directory is at on your computer.
   This defaults to `C:\streaming-automations\highlighted-message`.

Some other example triggers are provided. `Manually Highlight Message` can be
assigned to Streamer.Bot's Quick Action Bar in chat, or can trigger based on
Twitch highlighted messages. A queue holds all of the messages and displays
them one at a time.

You can automate the turning on and off of the queue via the `Disable Message
Highlights` and `Enable Message Highlights` actions. Example OBS scenes have
been provided.

The show/hide animations have been built into the browser source page to allow
for animations in the
[https://github.com/Aitum/obs-vertical-canvas/](obs-vertical-canvas) plugin,
which currently does not support scene item show/hide animations.
