#### Welcome to Pacman
```
python pacman.py --layout testMaze --pacman GoWestAgent
python pacman.py --layout tinyMaze --pacman GoWestAgent
```
#### Finding a Fixed Food Dot using Depth First Search / Breadth First Search
```
python pacman.py -l tinyMaze -p SearchAgent -a fn=tinyMazeSearch
python pacman.py -l tinyMaze -p SearchAgent -z.3 --frameTime=0.03
# -l {tinyMaze | mediumMaze | bigMaze}
# -a fn={bfs | dfs | ucs | astar}
python autograder.py
```
### DFS
> 深度优先遍历
> 1. 访问指定的起始顶点;
> 2. 若当前访问的顶点的邻接顶点有未被访问的, 则任选一个访问之; 反之, 退回到最近访问过的顶点; 直到与起始顶点相通的全部顶点都访问完毕
> 3. 若此时图中尚有顶点未被访问, 则再选其中一个顶点作为起始顶点并访问之, 转 2;  反之, 遍历结束

### BFS
> 从图的某一结点出发, 首先依次访问该结点的所有邻接顶点,  再按这些顶点被访问的先后次序依次访问与它们相邻接的所有未被访问的顶点, 重复此过程, 直至所有顶点均被访问为止.

## bfs＝队列，入队列，出队列；dfs=栈，压栈，出栈


### UCS
> 成本一致搜寻法（en:uniform-cost search）, BFS的改良算法
> 对一般的图来说，BFS并不一定回传最佳解。这是因为当图形为加权图（亦即各边长度不同）时，
> BFS仍然回传从根节点开始，经过边数目最少的解；而这个解距离根节点的距离不一定最短。
> 这个问题可以使用考虑各边权值，BFS的改良算法成本一致搜寻法（en:uniform-cos search）
> 来解决。然而，若非加权图形，则所有边的长度相等，BFS就能找到最近的最佳解。

### A*
> A-Star算法是一种静态路网中求解最短路最有效的直接搜索方法。
> UCS的改良算法 加上了估价函数，保证找到最短路径（最优解的）条件，关键在于估价函数h(n)的选取

## UCS 和 A* 都是队列，入队列，出队列，不同之处在于出队列的权重顺序




> Finished at 21:15:28

> Provisional grades
> ==================
> Question q1: 3/3
> Question q2: 3/3
> Question q3: 3/3
> Question q4: 3/3
> Question q5: 3/3
> Question q6: 3/3
> Question q7: 5/4
> Question q8: 3/3
> ------------------
> Total: 26/25
