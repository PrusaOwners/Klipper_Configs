# Prusa MK3 Klipper Config

## THIS IS A WORK IN PROGRESS AND HAS NOT BEEN VALIDATED YET!

If you are interested in contributing or testing then contact KenadyDwag44 on the Unofficial Prusa Discord or 602 Discord.

## About

This is yet another klipper configuration for the Prusa MK3. Unlike some others, this one is going to try and stay basic so that 
one can hit the ground running with a solid klipper config then add whatever they would like whenever they feel like it. I am hoping
to add most of the essential features that come from prusa firmware.

![](https://imgs.xkcd.com/comics/standards.png)


### NOTE! Prusa's fork of Marlin is heavily edited and optimized for their machine. 
This firmware will never be 100% the same as the markin version and will take a little more effort to run. But it is still real easy
and I believe in you :).

## How to use
    1. Install Klipper on your machine
    2. Clone or download the entire repo to the klipper machine.
    3. Make all the edits you need to in printer.cfg
    4. Use the following below inside of your slicer profile to take advantage  of the print start and end macros:

    Start G-code:
    M190 S0
    M104 S0
    print_start EXT_TEMP=[first_layer_temperature] BED_TEMP=[first_layer_bed_temperature]

    End G-code:
    print_end


## Work in Progress

- Testing, testing, and more testing
- Bed screws support to tune silicon mod and nylock mod
- More tuned filament sensor support




```yml
[update_manager prusa]
type: git_repo
origin: https://github.com/PrusaOwners/Klipper_Configs.git
path: ~/klipper_config
primary_branch: main
is_system_service: False
```
