[[Graph and Networking Algoriithms]]
[[Depth-first Search algorithm]]

## Javascript execution of the breadth-first searching algorithm

#### This is a searching algorithm that takes advantage of queues,  to go to every node. It searches in every direction equally.

const graph = {
 a: ["c", "b"],
 b: ["d"],
 c: ["e"],
 d: ["f"],
 e: [],
 f: [],
 }
 
** //depthfirstsearch recursion based
// const depthFirstPrint = (graph, source) => {
//     console.log(source)
//     for (let neighbor of graph[source]) {
//         depthFirstPrint(graph, neighbor)
//     }
// }
// depthFirstPrint(graph, "a") //acebdf**

  

const breadthFirstPrint = (graph, source) => {
 const queue = [source];
 while (queue.length > 0) {
 current = queue.shift();
 console.log(current);
 for (let neighbor of graph[current]) {
 queue.push(neighbor)
 }
 }
}
breadthFirstPrint(graph, "a")


#algorithms #networking 