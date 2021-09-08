# assignment2-malireddy
# Nithin Sai Reddy Malireddy
## HYDERABAD

HYDERABAD is best **place** for **living** . It's also called as land of **biryani's**

*****
# Trip from maryville to Hyderabad
1. Firstly book the cab by using uber App to kansas airport 
2. take a flight from kansas airport to Hyderabad airport
3. After reaching the destiantion take the cab and see historical places in hyderabad
    1. charminar
    2. golconda fort
    3. lumbini park
    4. Had my famous biryani
       1. chicken biryani
       2. mutton biryani
5. In below two places i enjoyed a lot
- nagarjuna sagar is very close to hyderabad
- neckalce road is famous for buddha

[Bio and Image](AboutMe.md)

*****
## Beverage Section
Famous drinks available in Arby's.
Beverage, location & Price

| Drinks    | Location | Price |
|------------|----------|-------|
| Pepsi     | Arby's| $2.00 |
| Diet coke | Arby's| $1.50 |
| Sprite    | Arby's| $1.80 |
| Powerade  | Arby's| $2.20 |

---
## Pithy Quotes
*Helen Keller* said:

> The best and most beautiful things in the world cannot be seen or even touched — they must be felt with the heart.

> Alone we can do so little; together we can do so much.

##  Code Fencing

**Breadth-First-search algorthim** form **Graphs Traversal**

> Breadth-first search (BFS) is an algorithm for searching a tree data structure for a node that satisfies a given property. It starts at the tree root and explores all nodes at the present depth prior to moving on to the nodes at the next depth level. Extra memory, usually a queue, is needed to keep track of the child nodes that were encountered but not yet explored.
> For example, in a chess endgame a chess engine may build the game tree from the current position by applying all possible moves, and use breadth-first search to find a win position for white. Implicit trees (such as game trees or other problem-solving trees) may be of infinite size.

Breadth-First-search algorthim [Reference link](https://en.wikipedia.org/wiki/Breadth-first_search)


 
code for Breadth-First-search algorthim
```
vector<vector<int>> adj;  // adjacency list representation
int n; // number of nodes
int s; // source vertex

queue<int> q;
vector<bool> used(n);
vector<int> d(n), p(n);

q.push(s);
used[s] = true;
p[s] = -1;
while (!q.empty()) {
    int v = q.front();
    q.pop();
    for (int u : adj[v]) {
        if (!used[u]) {
            used[u] = true;
            q.push(u);
            d[u] = d[v] + 1;
            p[u] = v;
        }
    }
}
```

Breadth-First-search algorthim [code_link](https://cp-algorithms.com/graph/breadth-first-search.html)