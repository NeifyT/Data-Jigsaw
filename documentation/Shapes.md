# Standard Shape Orientation

The following is a guide to methods I have used in the real world for large-scale puzzles to assist in visual scanning of pieces. While, other puzzlers may use totally different techniques, this app is designed for my use, and thus will feature tools to handle these with rapid position and rotation alignment.

## Designated Shapes and Orientations

In a standard fully-interlocking puzzle (without whimsy) each piece has four distinct sides, and generally all pieces are the same relative size. Each side would have either a tab or a blank to fit with the piece next to it. By categorizing each piece by how many tabs and blanks and their relative positions, I have found rotating pieces in a standard direction helps me visually scan across large quantities to find an exact piece.

Below you will find my arbitrary designations for each shape archetype, the numerical number will be stored in *piece.shape*.

### 1—Corners

![Four distinct corner piece shapes with a single designation.](images/piece-1.png)

This is a good point to reinforce that this app will not be dealing with unusual shapes. Each puzzle would be cut from a user-chosen image that is a rectangular shape with any aspect ratio.

That said, every puzzle will have exactly four corner pieces. The four distinct shapes for corner pieces may be randomly cut such that any puzzle may have one, two, three, or all four of the shapes. As there will only ever be four such pieces it stands to reason to designate them with one number (1) so an automated sort can pick those four pieces out instantly regardless of the tabs and blanks they feature.

### 2—Edges with two blanks

![Two edge pieces featuring two blanks connecting to other edge pieces.](images/piece-2.png)

Provided that I like to start with the border of the puzzle, I rarely pay attention to the inner connection tab or blank. My second designation focuses on the two edge connecting sides as both blanks.

Notice that the orientation is with the edge to the bottom regardless if any piece is a bottom, left side, right side, or top edge. Keeping them the same is faster to look at the left or right side for matching tab and blank connections.

### 3—Edges with blank on the left and a tab on the right

![Two edge pieces featuring a blank on the left and a tab on the right connecting to other edge pieces.](images/piece-3.png)

Again these two shapes are combined based on only the connections to other edge pieces. This is the first distinct scanning, knowing which side I am looking for either a tab or a blank I can skip over ones designated as #4 even if I still scan across pieces designated as #2 or #5.

### 4—Edges with a tab on the left and a blank on the right

![Two edge pieces featuring a tab on the left and a blank on the right connecting to other edge pieces.](images/piece-4.png)

Another obvious combination allowing me to skip over ones designated as #3 even if I still scan across pieces designated as #2 or #5 depending on if I am searching for a tab or a blank.

### 5—Edges with two tabs

![Two edge pieces featuring two tabs connecting to other edge pieces.](images/piece-5.png)

The last designation of edge pieces completes the pattern with pieces having two tabs that connect to other edge pieces. When four long lines of edge pieces (oriented with edges at the bottom) have been completed or mostly completed I rotate them to form the rectangular border.

### 6—Four blanks

![A simple puzzle piece shape with four blanks.](images/piece-6.png)

From this point on each piece has a tab or a blank on each side and will stand alone. As a child I affectionally called this four-blank shape a "star." I got that by focusing on the corners not the blanks. It is as if it were a four-point star.

Indeed, when I am searching for a piece that has two blanks next to each other my focus is on the shape of the corner not the blanks themselves. Thus, I scan across the stars (6), men (7), and wolves (8).

It may be noted that all 90 degree rotations are "standard" with this shape. To keep the app from giving away the final orientation in the puzzle it will randomly assign a rotation offset for using the standard orientation positioning tools.

### 7—Three blanks and one tab

![A simple puzzle piece shape with three blanks and one tab with tab on top.](images/piece-7.png)

Just looking at this piece you can easily see why this one received the name "man" from my childhood. I rotate this such that the tab is at the top as a head with arms sticking out to the sides and legs underneath.

At this rotation even if I am only working with a single tab and looking for a blank to connect it to, I can quickly scan the left, bottom, right blanks ignoring the top tab. This cuts visual scanning time down by a quarter. Or a 75% reduction time scanning for a tab, straight across the top. Knowing exactly where tabs and blanks are positioned leaves more time to focus on distinct shapes or color blends.

### 8—Two consecutive tabs and two consecutive blanks

![A simple puzzle piece shape with two tabs in a row and two blanks in a row scanning clockwise from the left.](images/piece-8.png)

No doubt if you read my description of #6 you are wondering why this orientation and how this is a wolf. For this technical documentation I have tried to start with blanks and move to tabs, but I didn't organize that way as a child. This orientation with tabs on the left and top followed by blanks on the right and bottom felt most natural to me. Coming up with a representation of the shape to a real-world object took more imagination. Imagine if you will a wolf facing to the right tail curling up and out behind him, his snout high in the air howling at the moon. Back paws are on the ground and front paws standing up in front. 

Okay that is a stretch, and you don't need to think of it as a wolf, but this is my standard orientation for that shape and for rapid visual scanning.

### 9—Two blanks opposite of each other and two tabs opposite of each other

![A simple puzzle piece shape with two tabs and two blanks on opposite ends and a tab on top.](images/piece-9.png)

In my childhood I called this one the "bed," as sort of as a bird's-eye view with the head of the bed on top. I didn't lay this horizontal because of the scanning technique. I scan tabs across the top and then across the bottom, which matches scanning tabs across the top of the men. If I am looking for blanks I just scan across the middle of each piece. Similar to the stars this piece could be standard orientation with two different rotations, which the app will randomly choose from.

### 10—Three tabs and one blank

![A simple puzzle piece shape with three tabs and one blanks with the blank on the bottom.](images/piece-10.png)

You may be able to guess my name for this archetype and orientation with tabs on the left, top, and right. This is the closest match to other orientations allowing scanning evenly. While this documentation tries to adhere to standard computer graphical notation starting on the top moving clockwise, my orientations are holdovers from childhood, where I generally start on the left side. Having given you a little time to guess, I will now reveal this as a camel with its feet on the ground a tail on the left, hump on top, and head to the right.

### 11—Four tabs

![A simple puzzle piece shape with four tabs.](images/piece-11.png)

The greatest of these pieces is the sun with eight rays around it (4 tabs and 4 corners). Like its cousins the distant stars (#6) this shape can be oriented four ways and remain standard. The app will randomly pick the standard rotation offset. 

It may be said that while I use this scanning technique with standard orientations, I don't necessarily build everything that way. When color shows the precise orientation I will often orient that way. For example, a piece bordering on sky and mountain I will turn it sky up. In such cases I would be scanning for lines of demarcation not so much for tabs and blanks.

## Orientation Mechanisms

In the real world organizing shapes, rotating them to a standard rotation, and laying them out in a grid pattern for rapid visual scanning can be quite tedious. Would be even more tedious with a drag-and-drop user interface. I generally would do them in small batches first sorting by color and working within a color set. The largest puzzle I completed was 6,000 pieces. When I got to a point of very dark greens to blacks spreading across nearly the entire bottom quarter of the puzzle, I laid them out this way across many cardboard slabs on my floor, over 1,000 pieces remaining just to finish it. This took a lot of physical space and even more patience, but it paid off.

The digital realm has no real limitations. The intent will allow mass piece selection (through different methods) and with a couple clicks of a mouse or key presses sort them by shape, orient them, and arrange them in a grid pattern. This will remove the tedious piece organization and manipulation allowing a user to focus on the challenge of finding and connecting pieces to build a larger picture.

To accomplish this automaticity two data attributes (*shape* and *rotation_offset*) are included for each piece. The *shape* is an integer from 1 to 11 as designated above. The *rotation_offset* will store degrees in increments of 90 degrees where 0 is the real orientation of the piece as it will fit in the puzzle and the offset is how many degrees to turn that shape to match the standard orientation.