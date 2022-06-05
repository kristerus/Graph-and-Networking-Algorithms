[[Graph and Networking Algoriithms]]

The Bellman-Ford algorithm, it's an enhanced version of [[Dijkstra's Algorithm]]'s algorithm, which can also work with edges of negative length value, although slower. The key is the RELAX operation, applied to the edge. In a single scan of the edges we execute the RELAX for each edge. The step is then repeated [node number-1] times. NO special data structures to implement this algorithm.
In js it would look like:


![[bellman_ford_algorithm.png]]

Starting from p->5-1=4 iterations


|Source|Length|Predecessor|
|------|------|-----------|
|P|0|P|
|Q|2|P|
|R|4|P|
|S|2|T|
|T|7|R|








#algorithms #networking 