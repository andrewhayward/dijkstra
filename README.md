# Dijkstra's algorithm

"Dijkstra's algorithm, conceived by Dutch computer scientist Edsger Dijkstra, is a graph search algorithm that solves the single-source shortest path problem for a graph with nonnegative edge path costs, producing a shortest path tree. This algorithm is often used in routing and as a subroutine in other graph algorithms."


```js
var map = {a:{b:3,c:1},b:{a:2,c:1},c:{a:4,b:1}},
    graph = new Graph(map);

graph.findShortestPath('a', 'b');      // => ['a', 'c', 'b']
graph.findShortestPath('a', 'c');      // => ['a', 'c']
graph.findShortestPath('b', 'a');      // => ['b', 'a']
graph.findShortestPath('b', 'c', 'b'); // => ['b', 'c', 'b']
graph.findShortestPath('c', 'a', 'b'); // => ['c', 'b', 'a', 'c', 'b']
graph.findShortestPath('c', 'b', 'a'); // => ['c', 'b', 'a']
```
