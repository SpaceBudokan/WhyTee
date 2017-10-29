# WhyTee
YouTube for commandos.
Version 0.1

WhyTee is a simple command line tool for people that think they are too good for mpsyt. It depends upon the Google API library for python. You also need to put your Google developer API key in at line 26. It let's you search for videos, search for related videos, and list a channel's videos. This is done exclusively from the command line, and results are sent to stdout. Each field is on a newline, and each video is seperated by an empty line. Be aware, that if you include the description in your results, it may contain newlines. It may contain lots of newlines.

Search strings containing spaces must be placed in quotes. Note that when getting videos for a specific channel, you must pass the 24 character channel ID, not the channel title. 
