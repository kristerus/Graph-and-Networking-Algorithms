[[Graph and Networking Algoriithms]]
[[Breadth-first Search algorithm]]

#### This is a networking algorithm that aims to find the desired node by going deep one direction at a time.

const graph = {
 a: ["c", "b"],
 b: ["d"],
 c: ["e"],
 d: ["f"],
 e: [],
 f: [],
 }
 
 //depthfirstsearch function based
 // const depthFirstPrint = (graph, source) => {
 //     const stack = [source]
//     while (stack.length > 0) {
//         current = stack.pop()
//         console.log(current)
//         for (let neighbor of graph[current]) {
//             stack.push(neighbor)
//         }
//     }
// }


#algorithms #networking