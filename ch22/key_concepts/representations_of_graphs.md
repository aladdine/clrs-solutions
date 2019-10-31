## Representations of graphs:
+ There are two ways to present a graph: in an adjacency list or adjacency matrix.
+ Density of a graph is measured by the relative ratio of number of edges with respect
 to vertices (|E|^2/|V|^2).

Adjacency List | Adjacency Matrix
--- | ---
takes V + E memory space | takes V^2 memory space
suitable for sparse graphs | suitable for dense graphs
checking if two edges are directly connected is more expensive | checking if two edges are directly connected is cheap

### Examples:

```
  0 -- 1
  |    |
  |    |
  2 -- 3 -- 4
```
#### Adjacency list:

```python
x = [
	[1, 2],
	[0, 3],
	[0, 3],
	[1, 2, 4],
	[3]
]
```

#### Adjacency matrix:

```python
x = [
	[0, 1, 1, 0, 0],
	[1, 0, 0, 1, 0],
	[1, 0, 0, 1, 0],
	[0, 1, 1, 0, 1],
	[0, 0, 0, 1, 0]
]
```