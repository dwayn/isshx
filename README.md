# isshx
Cluster ssh for iTerm2 

## Intro
I have used csshX for a while now and I love it, but a couple years ago I made the switch to iTerm as my primary terminal, so I built an equivalent tool for iTerm.

This is iTerm2 2.9+ compatible (the AppleScript API in iTerm changed significantly in 2.9). 


## Installation
The whole tool is just an AppleScript in the shell script `isshx`, so it can be copied or symlinked anywhere in your path. 

## Usage
isshx only needs a list of servers to ssh to:

`isshx SERVER_HOST [SERVER_HOST [SERVER_HOST [...]]]`

Once the new terminal window is open you can use iTerm's native support for broadcast to send input to all sessions in the window. By default, this `Cmd + Shift + I` to enable/disable broadcast. 

_Take note that when you enable broadcast to a window, it will enable it for all sessions in all subwindows as well as any session in other tabs of that particular window. This is why isshx creates a new window every time._
