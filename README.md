# Custom Vib Image for the Microsoft surface lineup with NVIDIA GPUs

This is a Vib Image to get the required linux-surface patches working on Vanilla OS, it's based off of the nvidia Vib Image from Vanilla OS.

## How can I get this?

Surprisingly simple, open the terminal and run `abroot config-editor` a file should open in nano (or any other text editor you have configured).
In the file change the `name` parameter to `sakloui/surface-nv`, then save and close. 
Then run `abroot upgrade` and wait for it to finish and reboot. you can check if it's working by opening the terminal and running `uname -a`, if the surface kernel is shown then it should be working.

## I don't want to get the nvidia drivers because I don't have a dGPU

I currently haven't made a Vib Image for this, but you can create a template from [https://github.com/Vanilla-OS/custom-image](here) follow their steps, and copy most of the config from this repo.
