# mpv-timer

## Description

A simple plugin for mpv which allows the user to set a starting time and an
ending time and see the time elapsed between those points with millisecond
precision. 

## Installation

Install the script by downloading the .lua file and placing it in your mpv
scripts folder or running the program as  
```mpv --script path/to/script.lua```

## Use

The program is used by navigating to the starting frame (using arrow keys, '.'
and ',' for frame advance or any other method of your choosing) then pressing
the start key, which can be bound in input.conf as  
```z script-message-to mpv-timer set-start-time``` 
and the end key, which can be similarly bound in input.conf as
```x script-message-to mpv-timer set-end-time```  

Once the program recieves a start and end time, it will calculate the total
elapsed time and print it to the screen for 5 seconds. After this time the user
can display it again by pressing a key bound as
```c script-message-to mpv-timer print-time```
