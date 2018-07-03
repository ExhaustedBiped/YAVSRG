Interlude is a rhythm game written in C#. You play it with a keyboard it supports some of the popular chart formats from other rhythm games. Interlude aims to combine the best features from other rhythm games and to create a platform that can be used equally casually and competitively.

## Hi

This will be the "check it out" section of the page soon, but there is no public release yet. It was supposed to be the 1st of July but I'm pushing it back a bit because it just isn't ready yet.
[Click here to see the repository and code](https://github.com/percyqaz/YAVSRG)

## What's the point of developing another rhythm game?

Interlude aims to compete with the most popular 4k rhythm games, Etterna (a branch of Stepmania 5) and osu!mania. This is because I (percyqaz) have found them lacking in certain features which in most cases are implemented by one of the two but not the other.

### Issues with osu!mania (the main ones)
* Star rating *sucks* and we're talking really bad. The PP system is notorious for favouring patterns like "jumptrills" rather than things that are either physically difficult or hard in context of a rhythm game such as technical rhythms or patterns of notes. This makes osu!mania almost useless for competitive play as your ranking is not very well correlated with ability in all areas.
* The editor for charts in osu!mania is fairly dated and is the bare minimum tool for creating charts. I would like to have an editor with many more tools, especially for things like scroll speed changes and pattern generators to speed up the workflow and also make charting accessible to more people.
* There is a fairly limited range of charts available that are ranked for osu!mania due to the "quality control" in place by human review. If I end up creating an online score system I would like to allow all scores to be saved online rather than just select charts. Stepmania has a much wider variety of charts simply because of age and are used to converting them to osu!mania even though they are not ranked and players cannot set global scores on them.

### Issues with Etterna
* There is no in-built chart editor, with popular external editors including DDReam Studio and ArrowVortex. These again do not have some features I'd like when working with charts. They also operate in the stepmania chart format, which is clunky and often not normalised or formatted correctly so I would very much like to get away from this file format for charts.
* Wife, the accuracy system for Etterna, is very harsh on misses while being notably more lenient on other signs of poor accuracy such as hitting a lot of "greats" instead of "perfects". I think it is too focussed on making sure players hit all the notes to be a good measure of rhythm or skill other than the physical skill of not missing. This may also be one of the root causes of issues with MSD rating for scores as a handful of misses will severely degrade your score even though your performance could really be much higher. (and this causes the MSD to be higher to compensate, causing broken scores when someone actually doesn't miss)
* There is no support for "long note" charts in stepmania, where a chart contains patterns of notes you must hold and release at the correct time in complicated patterns. Hold notes in Etterna act almost exactly like tap notes but look different, as the hold requirement is too lenient to be used as a challenging game mechanic.
* There is little to no support for "slider velocity" charts like in osu!mania where varying scroll speeds can be set during a chart to create visual effects such as teleporting notes, slow downs, bouncing effects, etc. I really like using this mechanic from osu!mania for adding extra interesting details to charts other than timing as this can change how players "read" or interpret the notes on the screen.
* While support for other keymodes exist in Stepmania, it is being phased out in Etterna, and MSD does not support keymodes other than 4 keys. I would like to create a good difficulty calculator for keymodes from 3k to 10k and am especially interested in having quite a large focus on 7k as it is a popular keymode and used in games such as LR2, O2Jam and IIDX.

## Features

You can read a more detailed plan of features [here](https://docs.google.com/document/d/1qMs9kOYra077usI3LIZ28-BaAVQY7y-Te-EilGAncqg/edit) but at the time of writing this, it isn't up to date or complete.
The plan is that you'll have enough to play either competitely or casually, the way you like :)

### We got..
+ Support for skins/themes where you can customise the appearance of the game and the notes you hit, including animations and a bit of flexibility in layout of the user interface.
+ Ability to convert charts from .osu (osu!mania) and .sm (Stepmania/Etterna)
+ Work in progress automatic chart difficulty calculator that gives you a performance rating and stores your scores - Read about it [here](https://docs.google.com/document/d/1sW1OGfcRdu8UL1duk66vNv96GaDKCUef5YrrpmZhMNs/edit)
+ New performance can be recalculated from old scores when the calculator is updated
+ Caching and searching of installed charts for fast loading speeds.
+ Support for hold note styled charts, slider velocities in charts and mines in charts
+ Support for keymodes 3-10
+ The ability to use "rates" - Speeding up or slowing down a chart to suit your skill level
+ A choice of either the notes scrolling up or down the screen (and some other stuff you might want like screencovers)

### We plan to implement..
+ A really good automatic difficulty calculator that beats out MSD (and less mentionably star rating)
+ Peer-to-peer online multiplayer and chat
+ A fully featured chart editor
+ An HP system where you can "fail" a chart by running out of HP due to missing too much
+ Collections and playlists of maps
+ Sound effects when you hit notes (but they won't be assignable to each note individually like keysounding in osu!mania or LR2)

### We might eventually implement..
+ Online multiplayer and score servers (If I can afford/get stable income to support it and enough people are interested)
+ Regular/weekly challenges for players to complete
+ Some more stuff hopefully, we'll see...