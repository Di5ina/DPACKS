# DPACKS
Repository for my free dpacks. These packs can be used with either the free or pro versions of simple scifi by Chipp Walters

## Install
open the simple scifi scene.  Go to File > Append, browse to one of these packs, and import the collection.
Simple scifi can be acquired here: [Free](https://chippwalters.gumroad.com/l/simplescififree), [Pro](https://chippwalters.gumroad.com/l/simplescifi)

Note these packs are under development and will change often.


## Packs
### Dots-P-GeoGenerative-01
This pack contains 10 copies of a geometry node network that creates window-like patterns. When using it feel free to delete copies for less overall variation or add more duplicates for more. Just remember that if you duplicate them you need to select a new seed for the copy. Options are:

* **Seed:** Create randomization. Make sure this is different for each layer
* **Window Length X:** larger values make the pattern wider. This value is subject to randomization so the windows will not necessarily reach this length.
* **Window Length Y:** Height of the pattern. No randomization.
* **Window Fill Probability:** This allows a random selection of windows to be 'skipped' simulating some of the lights being turned off.
* **Window Size:** controls how large individual windows are at default 1:1:1 scale.
* **Window Cluster Size:** controls the overall pattern size. Selecting smaller values will make everything smaller and reduce the space between windows, while making it larger will space everything out.
* **Circular Windows:** switched the window geometry from squares to circles.
* **Material:** This option does nothing within simple scifi and is mostly for testing.

### Dots-P-GeoGenerative-02
This contains a single copy of the geometry node from Dots-P-GeoGenerative-01 as well as two new nodes still under development

First is a node that generate windows in a concentric ring pattern.

Second is a single ring with windows exploding outward from the center or inward towards the center.