# DPACKS
Repository for my free dpacks. These packs can be used with either the free or pro versions of simple scifi by Chipp Walters

## Install
open the simple scifi scene.  Go to File > Append, browse to one of these packs, and import the collection.
Simple scifi can be acquired here: [Free](https://chippwalters.gumroad.com/l/simplescififree), [Pro](https://chippwalters.gumroad.com/l/simplescifi)

**Note** these packs are under development and will change often. They are currently being developed on Blender 3.0.1 and are not guaranteed to work on previous versions. As geometry nodes are currently undergoing a lot of development these nodes will be upgraded to the latest mainline versions whenever they are available at the expense of backwards compatibility.


## DPACKs
### Dots-GeoGenerative-InsertReady
This File contains copys of the generators in the Development file instantiated with some reasonable values. They can be used as is or customized by adjusting settings in the modifiers tab.

### Dots-GeoGenerative-Development
This file is the repository file for all the nodes I'm creating. If you want to add more or experiment this is your template.

For the sake of simplicity I will be referring to the dots as windows. They don't necessarily have to represent windows in a render but as I will be describing a lot of geometry I don't want there to be any ambiguity. There is also an option to override the windows with instances of geometry. This can be used with other simple scifi dpacks to instance geometry in interesting ways but the settings will usually need to be lowered. I also included a scaling input because instanced geometry can get messed up very easily.

### List of Generators
#### Random Lines
Simulates lines of windows on something like an office building. Lines of a random length radiate from the center creating a pattern with solid top and bottom lines and a broken or jagged profile on the sides.


#### Concentric
Concentric produces a series of rings with options for even spacing between the rings or random spacing.


#### Concentric-ngon
Options are almost identical to the concentric circle generator, however a resample option has been added. Allowing modifying a low poly circle into an ngon with many dots along the edges.


#### CircleExplosion
Starts with a ring and projects lines of windows outward and inward. Effect is similar to a solar eclipse.


#### Grid
Setting one or both dimensions to 1 can be used to make lines or single points. Otherwise will produce a brick of windows.



## Overall TODO

* create youtube video with a simple overview on how these nodes can be used
* create sweeping lines, arcs
* Add support for an anti fill set to black
* Port the generators to decal inserts for manual detailing with kitops
* Port my dot's generator that produces tileable output.