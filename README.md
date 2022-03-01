# DPACKS
Repository for my free dpacks. These packs can be used with either the free or pro versions of simple scifi by Chipp Walters

## Install
open the simple scifi scene.  Go to File > Append, browse to one of these packs, and import the collection.
Simple scifi can be acquired here: [Free](https://chippwalters.gumroad.com/l/simplescififree), [Pro](https://chippwalters.gumroad.com/l/simplescifi)

**Note** these packs are under development and will change often. They are currently being developed on Blender 3.0.1 and are not guaranteed to work on previous versions. As geometry nodes are currently undergoing a lot of development these nodes will be upgraded to the latest mainline versions whenever they are available at the expense of backwards compatibility.


## Packs
### Dots-P-GeoGenerative-01
This pack contains 10 copies of the _Random Lines of Windows_ generator. When using it feel free to delete copies for less overall variation or add more duplicates for more. Just remember that if you duplicate them you need to select a new seed for the copy.

### Dots-P-GeoGenerative-02
This contains a single copy of _Random Lines of Windows_ as well as two new nodes, _Circle Explosion_ and _Concentric_, which are still under development

Concentric generates windows in a concentric ring pattern.

Circle Explosion generates a single ring with windows exploding outward from the center and/or imploding inward towards the center.

For the sake of simplicity I will be referring to the dots as windows. They don't necessarily have to represent windows in a render but as I will be describing a lot of geometry I don't want there to be any ambiguity. There is also an option to override the windows with instances of geometry.

### List of Generators
#### Random Lines
* **Disable Output:** Turns off output similarly to disabling view port/render visibility.
* **Seed:** Create randomization. Make sure this is different for each layer
* **Window Length X:** larger values make the pattern wider. This value is subject to randomization so the windows will not necessarily reach this length.
* **Window Length Y:** Height of the pattern. No randomization.
* **Window Fill Probability:** This allows a random selection of windows to be 'skipped' simulating some of the lights being turned off.
* **Window Size:** controls how large individual windows are at default 1:1:1 scale.
* **Window Cluster Size:** controls the overall pattern size. Selecting smaller values will make everything smaller and reduce the space between windows, while making it larger will space everything out.
* **Circular Windows:** switched the window geometry from squares to circles.

#####TODO
* **Instance Override:** Instead of generating windows generate instances of certain objects or from collections
* **Use collection:** True: Instance from the collection listed below, False: instance from the object instead. Ignored unless Instance Override is set.
* **Collection**
* **Object**
* **Material:** This option does nothing within simple scifi and is mostly for testing.

#### Concentric
* **Disable Output:** Turns off output similarly to disabling view port/render visibility.
* **Seed:** Create randomization. Make sure this is different for each layer
* **Random Rotation:** spin the rings randomly to break up the pattern
* **Snap Random Rotation:** Makes it so the rings snap to a common rotation. This creates lines of windows moving outward from the center.
* **Randomize Ring Diameters:** If set the rings will have a random diameter somewhere between min and max. Overlapping may happen. If not set rings will be evenly spaced between min and max.
* **Ring Resolution:** Resolution of the circle, directly affects how many points there are.
* **Number of Rings:** Number of rings to generate
* **Window Radius:** How big are the dots. Try to set this number to be the same for all generators to get a somewhat consistent result. As a function of how the rings are generated the further out rings generate larger windows. This is technically a bug but will be an option whenever I figure out a fix.
* **Ring(s) Min Radius:** Minimum radius rings can appear in
* **Ring(s) Max Radius:** Maximum radius for rings
* **Density:** Density of windows. Lower values means more windows are absent

##### TODO
* **Instance Override:** Instead of generating windows generate instances of certain objects or from collections
* **Use collection:** True: Instance from the collection listed below, False: instance from the object instead. Ignored unless Instance Override is set.
* **Collection**
* **Object**
* **Material:** This option does nothing within simple scifi and is mostly for testing.

#### CircleExplosion
* **Disable Output:** Turns off output similarly to disabling view port/render visibility.
* **Seed:** Create randomization. Make sure this is different for each layer
* **Explode:** Generate lines of windows outward from the ring
* **Implode:** Generate lines of windows inward
* **Ring Resolution:** Directly affects how many windows are generated around the ring and thus how many lines go inward or outward
* **Implosion Resolution Divisor:** Divide the Ring Resolution by this number before generating inward lines. A value of 2 will generate half as many inward lines as outward.
* **Explosion Density:** Lower values means less windows going outward
* **Implosion Density:** Lower values means less windows going inward
* **Dense Ring:** Create a higher density ring where the explosions/implosions radiate from.
* **Dense Ring Multiple:** Multiply the ring resolution by this number
* **Window Radius:** How big are the dots. Try to set this number to be the same for all generators to get a somewhat consistent result. As a function of how the rings are generated the further out rings generate larger windows. This is technically a bug but will be an option whenever I figure out a fix.

##### TODO
* **Instance Override:** Instead of generating windows generate instances of certain objects or from collections
* **Use collection:** True: Instance from the collection listed below, False: instance from the object instead. Ignored unless Instance Override is set.
* **Collection**
* **Object**
* **Material:** This option does nothing within simple scifi and is mostly for testing.


## Overall ToDo
* generate previews of each modifier
* finish making the modifiers pass through so that multiple modifiers can be stacked on an object
* create a single dot node
* create a concentric n-gon node
* finish setting up preview workflow.
* create youtube video with a simple overview on how these nodes can be used
* create a standard node group for instancing objects/collections instead of windows.