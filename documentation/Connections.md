# Tracking Connections of Pieces

My first two thoughts about how to track pieces presented a conundrum. I thought of a tracking method what would be a lot of duplicated data with quicker lookups, or a method of small data with recursive lookups. Determined I should test both and benchmark the better method I wrote them down. However, it wasn't long before I abandoned both completely before even starting to code anything.

A second round of contemplating how to keep track of which pieces were connected resulted in the relational data idea. Each piece will store its relation with a numerical dictionary key. A dictionary of connections will be maintained in the following manner.

1. When two completely loose pieces are connected a new key will be appended to the dictionary containing a list of the two piece IDs that just connected. Each piece will store the key of their group.

2. When a loose piece is connected to a group of pieces (or vice versa) the loose piece ID is appended to the key's list and the key ID added to the piece.

3. If two groups are connected the smaller (by list length) of the two keys is popped with its list values appended (or extended) to the other key and piece IDs are iterated to change their connection key. In case of a tie the lower the index will be the combined key.

4. The puzzle is completed when the only connection key has a length equal to the number of pieces in the puzzle.

With this method at most the total number of pieces will be stored in the connections' dictionary. No need for data duplication or recursive lookups. In a large puzzle, say 10,000, it is conceivably possible that every loose piece will be connected to only one other causing 5,000 keys in the dictionary. While highly unlikely benchmark tests will see how well that works. Also, unlikely two halves of the puzzle completed will benchmark the final connection. Benchmarks across other more likely configurations will be conducted.

## Moving/Rotating Groups

Moving and rotating groups is a challenge yet to be addressed. Changes will be handled at the data layer and then rendered appropriately. 

...More to follow...