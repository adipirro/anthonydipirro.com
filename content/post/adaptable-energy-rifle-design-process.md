+++
date = "2013-11-14T20:55:32-04:00"
title = "Adaptable Energy Rifle Design Process"

+++


{{< youtube 3Tf1bEFpPp4 >}}

</br>

When designing the Adaptable Energy Rifle (A.E.R) there were numerous things I took into consideration.  At the top of that list were time and experience.  Going in I had zero experience using the Unreal Development Kit and only three months to put something together.  The goals I decided to lay out for myself were as follows: 

* Learn UDK
* Build complete A.E.R weapon functionality
* Build a level to show off and play with the gun

As with all game projects, there were many different things to consider while I was building the gun.  To make things easier to read, I will separate each portion of the design process.

## Gun Design
Going in I knew I wanted to create something new and interesting since simply creating an energy rifle would not have been very challenging.  The idea for the modifiable nature of the gun came to mind while I was playing Republic Commando and saw how the weapon in that game could be reassembled in different ways to achieve different weapon types.  Thinking further on the idea I realized that the reason different weapon types exists in the first place is to allow the user to adapt to the various situations they are put in.  Taking the keyword "adapt" to heart, I decided to design the most adaptable gun I could think of.  

I wanted to give the player as much adaptability as possible, but not overwhelm them, so I settled on using four different weapon attributes: Power, Accuracy, Fire Rate, and Number of Projectiles.  Opening up these attributes allows for various weapon types to be created by the player, both basic (Assault Rifle, Shotgun, Sniper) and...different (Multi-Projectile Rifles, Fast-Firing Shotguns).  My favorite thing to do was set the Damage/Accuracy to 0 and crank the Fire Rate up to its max which allowed the gun to fire indefinitely, but does no damage (could be good for covering fire).

The cool down system was decided pretty early on and was designed in a way where more powerful weapons would generate more heat.  Normally I hate cool down based systems like this because they take you out of the action so to address this I made the cool down rate faster than normal and allow the player to fire without pause, even while the gun is unstable, at the cost of the instability causing an explosion if they become too overzealous.

The idea for the crystals didn't come until much later in the design process when I realized the gun was too static on its own.  Just by playing around with it myself I realized that players would likely just find a specific setting they were comfortable with and stick with it.  Since I wanted players to be adapting and changing how they play more often, I added the crystals which either restrain the gun (raw crystals) or open it up to more powerful possibilities (flawless crystals).

The gun could probably use some balancing tweaks, but other than that I feel like it is very solid.

## Sound Design

I love playing with sounds.  I am also a bit of a stickler when it comes to how things sound so I wanted to make sure things sounded as good as they could.  I had never done actual sound design before this, so I ended up doing a lot of research into how sounds are created for other Sci-Fi projects (Ben Burtt was a big inspiration).  

The main hurdle I had to overcome was how to make something which sounded powerful and deadly at all the different fire rates.  The problem was with the higher fire rates since using large explosion-type noises need time to express themselves and when played in quick succession make it sound more like your computer is dying than anything else.  It took a lot of time, but I eventually was able to create a sound which I think works very well and achieves what I set out to do.  The resulting sound is a mixture of a nice, thick,  laser zap and a car passing by at high-speed (both of which I found online). 

I am really happy with the way the sounds turned out.  The only thing I would explore if given more time is a way to make the gun sound changed based on the weapon attributes. 

## Models, Textures, Effects

It is probably worth noting that going in I had zero experience with 3D modeling software or texture work (the gun and test corridor represent my 1st and 2nd models respectively).  Most of the textures I ended up finding online since attempts to create them otherwise proved futile.  

One thing I am proud of on the art side, however, is the various color effects.  The gun has an inherently customizable nature to it, and I wanted to open up more ways for that to be expressed.  Even though it is a pretty small touch in the grand scheme of things, I think it adds a lot to the gun.

Another thing I am happy with is the scope.  Originally it had been more of a traditional scope which ran along the top of the gun, but as time went on I realized I wanted it to have more of a Sci-Fi look.  This was eventually achieved when I was playing Borderlands 2 and decided Ireally liked the floating hologram sights on the Maliwan SMG's.  

Overall, the results are incredibly sub-par, but I feel like the art at least succeeds in informing the player about what the gun is and how it "works."

## Level Design

This is probably the weakest portion of the project, at least regarding what I feel could have been done in its stead.   The corridor was designed to make things look cool, but in hindsight, it would have been better to create something out of simple geometry which makes the player have to adapt to different situations.   Seeing as the sole purpose of the gun is to have players adapt, this was a failure on my part to realize what should be done.  I originally scrapped the idea since I didn't think I'd be able to put together A.I., but thinking about it some more I could have gotten away with simply putting together a more complex level with both tight pathways and large open spaces.

## User Interface

When building the user interface, I tried to keep things as neat and simple as possible.  There is a lot of information which the player needs to have access to, but it needed to be both out of the way and easily accessible when needed.

The most troublesome portion of the UI, which I encountered, was how to visualize the cool down.   For the longest time, the lower right-hand bar was the only indicator, but I found that when in combat you don't want to be taking your eyes off the center of the screen.  So to remedy this problem, I added the cool down meter around the reticule which I feel does a better job at informing the player during combat.  

If I had more time, I would have liked to move all or most of the user interface onto the gun itself.  That was the plan from the beginning, but complications ended up causing more trouble than it was worth, so I stuck with what I had.

---

Overall I am pretty happy with how things turned out.  Coming from a programming background, I found Unrealscript fairly easy to get into.  The Unreal Engine was a hard to get into at first, but once I figured it out, I had a great time using it.  If I had more time, I would have liked to add multiplayer to test the various ideas in my head about how players might adapt to various situations.  

That about wraps it up.  There are probably some other small things I could touch on, but I don't want to bore you too much.  If you managed to make it this far, I applaud you and would like to thank you for your time.