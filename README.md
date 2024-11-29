# Lisa-Twiggy-Breakout-Board
A fork of Roland Juno's original Lisa breakout board - now with Twiggy!

![top](https://github.com/user-attachments/assets/b03664d9-7c32-4c2d-a7a4-0f4b118a8fd0)
![bottom](https://github.com/user-attachments/assets/54ac91fc-9dcd-4052-a664-bea79c118606)


# So... What is it? 
This is a variant of RolandJunos original Lisa breakout board (https://github.com/RolandJuno/Lisa_Breakout), that includes an additional connector for the Lisa LITE. 
Adding the Lisa LITE connector will allow for 400K Floppy Drives to be connected to a Lisa.
This is because the Lisa LITE generates a PWM signal for the main drive motor in the 400K floppy drive. 
In a Macintosh, this PWM signal is generated by the ASG and audio interface! (I mean, I guess it's all PWM signals).

However, 800K drives and Floppy Emu generate their own PWM signal - so that pin is usually left disconnected. 
As a result, you can use a passive adapter for those drives.

Note, in the surprising event that you have an actual Twiggy Drive, please note this probably will not work.
This is because to two signals (sense and read) are tied together for the 800K drive. I felt a bit lazy and didn't add a way to keep these separate. 
If you have a Twiggy, cut and strap I guess? 

# Engineers Notes
The BOM remains the same as the original breakout board, except for the addition of a 26 pin shrouded connector for the Twiggy pinout.

**IMPORTANT:**

Do NOT connect a Twiggy/Lisa LITE at the same time as a Sony Drive. They share the same enable lines, and bad stuff (TM) is likely to happen. 
So don't do that. 

**Errata and other notes:**

I've cleaned up some of the tracks and added thermal relief for soldering. 

The errata for the 7905 footprint has been fixed (and added some silk to make sure the polarity is right!).

AGND is also now connected to normal DGND, so no jumper is needed.

Mounting holes have now been added (three in total), which are positioned in a line on the board. This will help with case building. 

**NOTE - This is Entirely Untested. Proceed With Caution**

