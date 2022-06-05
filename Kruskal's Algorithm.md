[[Graph and Networking Algoriithms]]


In difference from the [[Prim's algorithm]], this algorithm grows not a single tree, rather a forest. 
1. edges are sorted in nondecreasing order of their costs. 
2. The algorithm starts with teh empty spanning forest.
3.  The edges are scanned in sorted order and if the addition of the current edge does not generate a cycle in the current forest, it is added to the forest.
4.  The main test at each step:
- Does the current edge connection between to vertices inthe same connected ocmponent.
- Eventually, the algorithm adds together [V]-1 edges to make a spanning tree.
5. An abstract version of this problem is known as the union-find problem for a collection of disjoint sets. Efficient alforithms are known for this  porblem, where an arbitrary sequence of UNION AND FIND operations can be implemented to run almost in linear time.

The code:
T<- fi
for v in G do
	Makeset(v).
for e=(u,v) in G //(in sorted order)// do
	if (u)!==(v)then
	T<-T U (u,v).
	Union(u,v).
end-proc

Time complecxity- >E *log E
![[kruskals-algorithm1.png]]

Starts from the smallest edge. A-B
Picks another not-related edge. C-D
Adds A-E, B-C and there it is.


#algorithms #networking #minimaledgesum #MST