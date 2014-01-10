Physics
=======

This is the testing ground for possibly integrating a physics engine into THREEx.  I have chosen to work with JigLibJS2 because it is relatively lightweight (a lot smaller than ammo.js, and just slightly bigger than Cannon.js).  Unlike cannon.js however, JigLibJS2 offers terrain (heightfield mesh) collision out of the box.  I feel that this is a very important part of wanting to add a physics engine in the first place.  The possibilites for games are great with terrain support.

Demo
----
Here's a demo of the integration with the latest version of three.min.js:

Drive the car with Arrow keys.  Click on objects to toss them up into the air.

Integration with Three.js
-------------------------
The authors of Three.js have changed some method names and functionality since JigLibJS2 was built.  Therefore, I had to alter how the demo calls certain functions.  I think I got everything working now. :)

Stability
---------
So far as engine stability is concerned, we will have to tweak and fine-tune the parameters for JigLibJS2.  I have done so in the above demo.  If the parameters are not tweaked, the demos can look buggy and unstable (stuff jumps around for no reason).  Therefore, part of this repo's effort will be to fine-tune as much as we can, so that when this engine is a part of THREEx (hopefully), then the user will just call the functions like new JBox, new JCar, startSimulation, etc., and it will run as expected with minimal jumpiness.

Maybe we can have physics 'presets' like outer-space, Earth-gravity, Jupiter-gravity, slippery ice, water, etc.
