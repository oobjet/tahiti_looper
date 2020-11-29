# Tahiti Looper
> a multiple synchronized live looper built with max


### Features

Tahiti Looper is a looper software.

#### Record, overdub and be cool

Download and launch Tahiti Looper.

Choose how many beats your first loop contains (you can think of them as slices of your loop or 1/8th notes).

Choose the maximum number of loops playing at the same time.

Press the Palm Tree button to start recording your first loop.

Press the Palm Tree button to stop recording your first loop and play it.

It plays again and again (it's a damn looper !).

Press the Palm Tree button to start recording of your second loop.

Press the palm Tree button to stop the recording of your second loop.

It automatically has the length of the closest multiple of beats of your first loop (you're a damn musician !).

Press and press again to record many other loops. When the maximum number of loop is reached, the first loop is silenced and then the second loop and then… OK, got it ?

Give it a try.

#### Simple, yet Powerful

You can start playing live-looping pieces of music that EVOLVE. Not always the same rythm with the same length. But it still stay perfectly SYNCHRONIZED. You can choose the DENSITY (number of loops) and the GRANULOSITY (number of beats).

A good example of what you can do is my own version of Terry Riley's IN C : [in c](https://objet.bandcamp.com/album/in-c-2) 

#### Additional controls

At the bottom right of the Plam Tree, Tahiti Looper tells you in wich state it is :

- reset : looper is stopped. No sound.
- record 1st loop : after a reset, records you intial loop wich will define the length of a beat
- play : it does only this. No recording of what you are playing.
- overdub : it adds a new layer of sound
- rest-armed : after a long press, the looper is ready to go back in reset state when you release the button

At the bottom of the window, you get a audio preferences button that open a window in which you can choose wich device (sound card) to use and wich channel inputs to record.

Next to this _audio preferences_, there's a tiny speaker that acts like a audio on/off button just in case something wrong happens ;-)

#### Want Tahiti Looper ?

Available for macOS & Windows.

Download [Max](https://cycling74.com/downloads) at cycling74.

Download or clone this repository.

Open TahitiLooper.maxproj

[![logo](/media/logo.png)](http://bit.ly/TahitiLooperV01)

## Why the world needs another looper

> The reason why I write another live-looping software, even though there're already too many audio loopers in this world.

### Infinite overdubbing goes the wrong way

Most loopers overdub layers of sound and you end up with wall of sound wich could be your style but is quite limited if we speak of composition.

With **Tahiti Looper** the rule is *first in first out* (known as FIFO). The oldest layer should go when there enough layers of sound running together (and you decide how many layers you tolerate).

This way you can make your piece evolve.

### Polyrythms are cool

.. and they should be easy to achieve. 

With **Tahiti Looper**, a new added loop is automaticaly a multiple or a divison of the original loop. It doesnt have to be the same length over and over and over…. but it could be.

Welcome 5/12 or 6/7 !

### Too many options are distractive

*Or the one button philosophy*.

Two many options mapped on too many buttons means that your music performance is transformed in a tap dancing show if your hands are on your instrument (which is probably the case if you play guitar like i do).

One button is enough because **Tahiti Looper** knows what to do at each tap (start a recording, stop another, play a loop and so on).

### Erare humanum est

And the machine should compensate for your mistakes.

**Tahiti looper** integrates a very special technology (known as *beat attraction*) that rounds up your slightly misplaced push of of button and is smart enough to always delivers a perfect timing when yours is not that perfect ;-)

### Inspired by 'In C'

I'm a musician and I play with live-looping for more that 20 years. I practically used every loopers made. My favorites were Echoplex Digital Pro and DL4.

One day I had a dream : play infamous Terry Riley's In C with live-loopers. Since I wasnt' able to do that with software, I decided to build one. It eventually became **Tahiti Looper**.

## FAQ

*How do I stop the damn thing to play ? How do I reset the looper ?*

A long press (>0,5s) on the palm tree button should put it in "reset-armed" state. For a perfect stop, it actually stops when you released the button.

*I play guitar, I can't play and press the button at the same time ? Footpedal ? Midi ?*

Yes ! You can link the palm button to any midi capable device. Note 36 or C-1 (*note on message*) on chanel 1 press the button. *Note off message* of the same note depress it (very imortant to tell short press from long press). All you have to do is to choose your midi interface in the menu at the bottom. If it does not appear in the menu, press midi button on the left to scan for your midi devices.

*What if I have too much output volume ?*

Reduce the sound level at the input. Tahiti looper does a simple addition of all track volume.

*How many looper can play together ?*

Sky is the limit. Or more precisely, your computer RAM is the limit.

*Why is it called Tahiti looper ?*

Because Tahiti is the place where I live !

*Sometimes, when I record a short loop, it doesn't play it. Bug ?*

No that's a perfectly normal behavior. If you try to record a loop that is way shorter than the length of a beat, it ignores it. Raise the *number of beats in the first loop* parameter (double it is a good starting point).

*Sometimes, when I record a loop, it is not exactly syncronized on the right beat. Bug ?*

If the *number of beats in the firt loop* parameter is too high and you first loop is quite short, you have to be very precise to get Tahiti Looper to find the right beats to close the loop. Try to lower this paramater or play a longer loop.
