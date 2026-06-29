# Containers

No good puzzle app design would be complete without a method of narrowing down the field of pieces to work with at any time. As a child my family would use bread pans as bins while sorting (usually by color). These quick containers with a high wall kept the pieces from scattering, and we had plenty (a dozen or so) to borrow from the kitchen.

The biggest problem with them was that pieces couldn't be laid out. For puzzles, I soloed I often used flattened cardboard boxes for larger puzzles or even the top and bottom of the box the pieces came in for smaller puzzles. This allowed space to turn pieces right-side up and spread them into a grid organization.

## Data Structure

The container data structure is going to mirror the working desktop canvas. A container may be opened either overtop of the desktop or in another window (especially with multi-monitor support). See [Desktop Canvas](/documentation/Canvas.md) for more details regarding rendering.

Containers can be designated as storage bins only, basically just a random pile of pieces to be worked on later. Or, they can be organized with grid patterns. Pieces can be connected to each other inside of containers.

## Number of Containers

While [Microsoft Jigsaw](/documentation/MSJigsaw.md) only provides three containers, it is anticipated that larger puzzle builds may need dozens to efficiently sort smaller amounts to work with.

## Key Bindings

Trying to drag pieces one at a time into one or more containers is a poor user interface mechanism. Moving pieces to a container should be as easy as pointing at it with a mouse and pressing a key. The mouse can be moved over pieces in rapid succession while number keys can be tapped to move pieces in. A flag in the settings can be toggled to either pile pieces or lay them out in a grid pattern.

The number keys (1-0 above the letters or 0-9 on the ten key) will provide access to ten containers at a time. Pressing Ctrl+# will activate any given set of ten; providing 100 distinct containers to sort into. We will call these layers of containers.

When viewing a container on any active layer using Alt+# will swap the active container with the same numerical placement of one on the tapped number layer. This way containers can be moved between layers, so pieces from one container can be sorted into containers from a different layer, given only one layer of ten containers is active at a time.

I anticipate even on a puzzle with 10,000 or more pieces; 100 containers would be enough to bring any section of the puzzle to a workable system.

## Auto Sorts

While I personally like the challenge of sorting pieces visually, with 10,000 pieces or more even this could become tedious. To conduct testing some automated tools will be developed as part of test scripts. These tools may be "cheating" in a way but will be provided for the user.

Actually, from what I have read it is quite common for extremely large puzzle builds to be bagged into smaller sections for completion anyway, so it may not be cheating by much.

Auto sorts will include:
- Sort by section
- Sort by shape
- Sort by color

These may be applied to all loose pieces or selected pieces not already connected.

### Sort by Section

If one were to take a 10,000-piece puzzle and sort by section specifying 100 sections; pieces would be placed into the 100 containers such that there would be 100 mini (100-piece) puzzles in each container. These could be assembled in their container then moved out to the desktop canvas to be assembled with each other. Or any similar configuration.

### Sort by Shape

An example of sorting by shape may be as simple as finding all edge pieces. Edge pieces sort to container 1, all others into container 2. One click and edge pieces for a 10,000-piece puzzle all in one stack. They can be dropped back on the desktop canvas and assembled.

Additional shape sorts would be based on the shapes described in more detail in the [Standard Shape Orientation](/documentation/Shapes.md) document.

### Sort by Color

The sort by color could prove more challenging to engineer. While I may experiment with finding color profiles based on pixel color counts and averages (mean, median, mode), I suspect that many types of images will not work out too well that way.

I am leaning to idea of adding AI features to this app in the future, passing the image and image fragments (found on each piece) through a convolutional neural network to handle image recognition.