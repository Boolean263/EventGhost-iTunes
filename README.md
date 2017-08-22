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

Events triggered: track changed, web radio stream track changed,
playback stopped.

## Downloads and Support

This plugin first appeared in
[this thread on the EventGhost forums](http://www.eventghost.net/forum/viewtopic.php?f=10&t=1815&start=0),
and that thread now serves as its support and distribution thread.
All releases so far have appeared as attachments to comments on that
thread. I'll do the same with my contributions.

I've copied the
[0.1.11 release](http://www.eventghost.net/forum/viewtopic.php?f=10&t=1815&start=45#p19716)
from that thread and used it to seed the GitHub repository at
[Boolean263/EventGhost-iTunes](https://github.com/Boolean263/EventGhost-iTunes)
(it's the initial commit there).
I make no claim of this repo being anything close to official;
that said, the thread has seen little to no activity in the last 2 years.

## Authors

Stottle, Jitterjames, cfull1, and now, Boolean263

## Changelog

### 0.1.13 - 2017-08-22

* [Release link](http://TODO)
* Refactor CallThread() so it works when iTunes isn't running
* Add a notice when the requested playlist name can't be found

### 0.1.12 - 2017-08-18

* [Release link](http://www.eventghost.net/forum/viewtopic.php?f=10&t=1815&start=60#p47694)
* Boolean263 dusts off the code
* New action: Play/Pause toggle
* Improve TrackChanged event: add kind, composer, comment, and genre
  to the payload
* Add StreamTrackChanged event: gives title and URL when a radio stream
  changes its title
* Add Stopped event when iTunes is stopped
* Some backend refactoring

Details below this line are a bit shaky.

### 0.1.11 - 2011-10-15
* [Release link](http://www.eventghost.net/forum/viewtopic.php?f=10&t=1815&start=45#p19716)
* Finally update the version number
* Clean up the code a bit
* Handle some error conditions
* Add "Play song in playlist" action

### 0.1.10 - 2011-10-10
* [Release link](http://www.eventghost.net/forum/viewtopic.php?f=10&t=1815&start=45#p19626)
* cfull1 joins the development
* Add repeat control
* Add info retrieval actions: shuffle, repeat, playlists, current playlist,
  playlist's tracks

### 0.1.10 - 2011-06-09
* [Release link](http://www.eventghost.net/forum/viewtopic.php?f=10&t=1815&start=30#p18478)
* Add "Search and Load" command: create a playlist and populate it with
  songs that match search terms
* Add shuffle control

### 0.1.10 - 2009-09-10

* [Release link](http://www.eventghost.net/forum/viewtopic.php?f=10&t=1815&start=15#p10597)
* No details given

### 0.1.10 - 2009-08-27

* [Release link](http://www.eventghost.net/forum/viewtopic.php?f=10&t=1815#p10224)
* Added ability to load playlist by name

### 0.1.10 - 2009-08-23

* [Release link](http://www.eventghost.net/forum/viewtopic.php?f=10&t=1815#p10125)
* stottle joins the development
* Added multithreading

### 0.0.1 - 2009-08-19

* [Release link](http://www.eventghost.net/forum/viewtopic.php?f=10&t=1815#p10027)
* Initial release by jitterjames
