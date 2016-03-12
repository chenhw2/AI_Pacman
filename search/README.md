#### Welcome to Pacman
```
python pacman.py --layout testMaze --pacman GoWestAgent
python pacman.py --layout tinyMaze --pacman GoWestAgent
```
#### Finding a Fixed Food Dot using Depth First Search / Breadth First Search
```
python pacman.py -l tinyMaze -p SearchAgent -a fn=tinyMazeSearch
python pacman.py -l tinyMaze -p SearchAgent -z.3
# -l {tinyMaze | mediumMaze | bigMaze}
# -a fn={bfs | dfs}
```
### DFS
> 深度优先遍历(DFS)
> 1. 访问指定的起始顶点;
> 2. 若当前访问的顶点的邻接顶点有未被访问的, 则任选一个访问之; 反之, 退回到最近访问过的顶点; 直到与起始顶点相通的全部顶点都访问完毕
> 3. 若此时图中尚有顶点未被访问, 则再选其中一个顶点作为起始顶点并访问之, 转 2;  反之, 遍历结束

### BFS
> 从图的某一结点出发, 首先依次访问该结点的所有邻接顶点,  再按这些顶点被访问的先后次序依次访问与它们相邻接的所有未被访问的顶点, 重复此过程, 直至所有顶点均被访问为止.

