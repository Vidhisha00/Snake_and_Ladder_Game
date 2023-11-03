# Snake_and_Ladder_Game

Snake and Ladder is a board game in which the roll of a dice determines how a player's counters advance along a grid. A ladder will lead you to a square that is closer to the end of the game, while a snake will force you back to a square that is closer to the beginning.

Here as an output, the least number of movements necessary to achieve victory in the game is determined for each individual cell. The user is presented with the option to modify their board or utilise the default board. Additionally, they are prompted to input the number of players involved in the game, which can be set to two, three, or four.

The idea is to consider the given snake and ladder board as a directed graph with number of vertices equal to the number of cells in the board. The problem reduces to finding the shortest path in a graph. Every vertex of the graph has an edge to next six vertices if next 6 vertices do not have a snake or ladder. If any of the next six vertices has a snake or ladder, then the edge from current vertex goes to the top of the ladder or tail of the snake. To find the shortest path we used Breadth First Search (BFS) of the graph. The topics used in this code are graphs, linked list, queues, and arrays.

