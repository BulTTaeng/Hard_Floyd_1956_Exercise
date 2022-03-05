# Hard_Floyd_1956_Exercise

made by Jaehyeok Choi

## Welcome to Jaehyeok's github!

## What is the problem?

![image](https://github.com/Choi-JaeHyeok-21500749/Hard_Floyd_1956_Exercise/blob/main/1956_pro.PNG)

## What Algorithm should I use?

Graph Algorithm , floyd - warshall

## What was the key point and the hard part?

At first , I use priority queue and pop smallest edge and if we detecte a cycle(visit already visited location and that location is starting node), that would be the answer.

However, there is no proof that that dfs got min value of cycle, because it might detect a bigger cycle first.

for example

1 -> 2 = 2;
2 -> 3 = 1;
2 -> 1 = 3;
3 -> 1 = 3;

In this case 2->3 will go first.

After that 1->2 goes in and 2->1 may goes in first.
Then it will say that there is 1 ->2 -> 1 cycle and it's cost is 5.

However , 1->3 ->1 is samller cycle(4).

So, I think another solution.

The problem is that I though floyd-warshall may work, but I don't know that floyd-warshall can find node - node(myself) distance.

Just using floyd warshall and find min value of node- node distance(dis[i][i]) will work.



## Where can I get more help, if I need it?

You can contact me through email, which is wogur7496@gmail.com.
Thank you for visiting this github!
