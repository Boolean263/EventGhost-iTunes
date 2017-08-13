# EventGhost-iTunes

This program is not very useful on its own. It's a plugin for
[EventGhost](http://www.eventghost.net/).
EventGhost is an automation tool for MS Windows
which listens for events -- whether user-triggered (like the press of a hotkey)
or system events (such as the screensaver activating) -- and runs actions
you specify. (It's like [Tasker](http://tasker.dinglisch.net/) for Android, or
[Cuttlefish](https://launchpad.net/cuttlefish) for Ubuntu.)

## Disclaimer

I (Boolean263) am not the original author of this code. It's a collaboration
of people on the EventGhost forums who go by Stottle, Jitterjames, and cfull1.
The official thread for this plugin is
[here](http://www.eventghost.net/forum/viewtopic.php?f=10&t=1815&start=0).
I've just put it here on GitHub because (a) I want to make it easier to find,
and (b) I want to start hacking on it myself.

## Description

This is a very handy plugin for EventGhost. It sends events on various changes
of iTunes state, allows you to retrieve various bits of information on the
state of iTunes, and even lets you control iTunes.

Simple control features supported: launch iTunes, exit iTunes, play, stop,
pause, next/previous track, rewind, fast-forward, resume, toggle
visualization/fullscreen/mute/shuffle/repeat, turn shuffle on/off,
turn repeat on/off/repeat all.

Advanced control features supported: set/change volume, load playlist
by name, search for songs and put them in a playlist, play a song in a
playlist.

Information retrieval fields supported: get title, album, artist, genre,
playlist name, playlist shuffle status, playlist repeat status, list of
playlists, playlist tracks by name, and "universal" (song name, album name,
artist, bitrate, BPM, comment, compilation, composer, date added).

## Downloads and Support

This plugin first appeared in
[this thread on the EventGhost forums](http://www.eventghost.net/forum/viewtopic.php?f=10&t=1815&start=0),
and that thread now serves as its support and distribution thread.
All releases so far have appeared as attachments to comments on that
thread. I'll do the same with my contributions once I feel they're worthy.

I've copied the
[0.1.11 release](http://www.eventghost.net/forum/viewtopic.php?f=10&t=1815&start=45#p19716)
from that thread and used it to seed the GitHub repository at
[Boolean263/EventGhost-iTunes](https://github.com/Boolean263/EventGhost-iTunes)
(it's the initial commit there).
I make no claim of this repo being anything close to official;
that said, the thread has seen little to no activity in the last 2 years.

## Authors

Stottle, Jitterjames, cfull1, and hopefully some day, Boolean263

