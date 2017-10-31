# WhyTee
YouTube for commandos.
Version 0.1

WhyTee is a simple command line tool for people that think they are too good for mpsyt. It depends upon the Google API library for python. You also need to put your Google developer API key in at line 26. It let's you search for videos, search for related videos, and list a channel's videos. This is done exclusively from the command line, and results are sent to stdout. Each field is on a newline, and each video is seperated by an empty line. Be aware, that if you include the description in your results, it may contain newlines. It may contain lots of newlines.

Search strings containing spaces must be placed in quotes. Note that when getting videos for a specific channel, you must pass the 24 character channel ID, not the channel title. 

Here is the output of "yt -h"
```

usage: yt [-h] [-t] [-u] [-U] [-i] [-d] [-c] [-C] [-D] [-l] [-T]
          [-m MAX_RESULTS] [-s | -a | -r]
          N

YouTube for commandos

positional arguments:
  N                     Search Terms, User, or video ID to search for.

optional arguments:
  -h, --help            show this help message and exit
  -t, --title           Display titles of results
  -u, --url             Display short url of results
  -U, --url_full        Display full url of results
  -i, --video_id        Display 11 character ID's of results
  -d, --description     Display descriptions of results
  -c, --channel_title   Display channel titles of results
  -C, --channel_id      Display channel ID of results
  -D, --date            Display dates results were published
  -l, --length          Display video length. NOTE: This requires an extra API
                        call
  -T, --thumb           Display URL of thumbnails of results
  -m MAX_RESULTS, --max_results MAX_RESULTS
                        Number of videos to return (default=10)
  -s, --search          Perform search using N
  -a, --channel         Returns videos for a specific channel ID, NOT channel
                        title.
  -r, --related         Returns videos related to ID

```
