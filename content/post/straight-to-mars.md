+++
date = "2016-06-14T20:31:32-04:00"
title = "Straight To Mars - A VR Experience"

+++

This summer I took part in Nexient's 2016 "Game of Codes" Hackathon event with a group of co-workers (Nathan Thomas, Atif Faiyaz, Jeffery Reichel, and Stewart Levine). Looking to have a little fun and take a little departure from our day-to-day tech stacks, we set our sights on Mars. 

Well, as close as you can get in 48 hours and $0.

Utilizing NASA's APIs, the Unity game engine, and Google's VR tools, we were able to create a convincing VR representation of Mars. Here are a couple of 3D screenshots from inside our app to give you an idea of what it looked like. 

{{< vrview "https://i.imgur.com/b0jDVKI.jpg" >}}

{{< vrview "https://i1378.photobucket.com/albums/ah109/Anthony_DiPirro/_2016-06-05_14-44-15-260_zpslwch3djv.png" >}}

The first step to procedural generation involved pulling grayscale altimetry data from NASA's public API's. This data was collected as part of their [MOLA](http://mola.gsfc.nasa.gov/) mission which launched back in 1996.

{{< figure src="/img/straight-to-mars/img1.png" title="Raw MOLA Data" >}}

Once the data is received, we move on to building out our mesh. The mesh generation starts by creating a "vertex cloud" based on the grayscale level of each pixel in the altimetry data. Once this "cloud" is created, we are then able to connect the vertices with triangles to form our final mesh.

{{< figure src="/img/straight-to-mars/img2.png" title="Generated Mesh" >}}

Now that we have our mesh...we want to spruce it up with a little bit of color. The texture data is pulled from another NASA API, this one serving up data from the [Viking](http://nssdc.gsfc.nasa.gov/nmc/spacecraftDisplay.do?id=1975-075A) mission launched in 1975.

{{< figure src="/img/straight-to-mars/img3.png" title="Viking Textures Applied" >}}

---

You can download the app yourself using the following link. Just make sure you hit the link on a Google Cardboard capable Android device. 

http://dl.anthonydipirro.com/VRMarsExploration.apk

**Controls**

Hold the button on your cardboard device to move in the direction you are facing. Just don't get any ideas about flying around, gravity is still a thing on Mars.

Double tapping the button will drop you in a random, new, pre-selected area of Mars. Loading time is about 40sec depending on the speed of your device. Not a lot of time for optimization!

