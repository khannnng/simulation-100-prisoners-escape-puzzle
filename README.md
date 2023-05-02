# simulation-100-prisoners-escape-puzzle
Simulate the strategy for the "100 Prisoners Escape Puzzle" proposed by Prof. Peter Bro Miltersen's.

(Original puzzle: https://www.youtube.com/watch?v=iSNsgj1OCLA&t=0s&ab_channel=Veritasium) 

### Problem:

Says there are 100 prisoner, numbered from 1 to 100:

![image](https://user-images.githubusercontent.com/112837341/235636765-4e804965-7467-47eb-b57b-7b694bc5dbc0.png)

And there are slips of papers contain their number, from 1-100 are randomly hidden in boxes, also labeled 1-100:

![image](https://user-images.githubusercontent.com/112837341/235636863-3f33d7f4-cf97-490b-a6f6-e64480371e60.png)

All the boxed are kept in a sealed room. Each of the prisoner are allowed in the room and search for their number by opening any 50 boxes.

![image](https://user-images.githubusercontent.com/112837341/235637277-12d89159-6418-41fb-85b7-ae6ac5a93c60.png)

And afterwards, they must leave the room exactly as they found it and exit the room. The next prisoner enters. They can't communicate to each others after they already entered and exit the room.

![image](https://user-images.githubusercontent.com/112837341/235637355-7f909586-98a8-4383-bb75-fa79fb339780.png)

If all 100 prisoners can find their number, they will be free.

![image](https://user-images.githubusercontent.com/112837341/235637405-061117b0-6f5f-45a8-8238-24bd26fb14b9.png)

But if even one of them can't find their number, all of them will be executed.

![image](https://user-images.githubusercontent.com/112837341/235637474-3481b6a8-ea3f-4a3b-92bb-4eb72fae4e2c.png)

If all of them open the 50 boxes at random, there probability of surviving is: 0.5^100 = 7.9e-31, pretty much non-existent.

The prisoners are allowed to strategize before and only before they start to enter the room. Is there a strategy to increase their probability of success?

![image](https://user-images.githubusercontent.com/112837341/235637546-00611b74-1b61-4b09-aa94-ffa9975b22dc.png)

### Solution
Please see explanation in the notebook or the original video.

### Coding simulation
This project is not the math for the probability in the answer, but the simulations to see if the probability checks out.

- First 2 attempts are proof of concept, which confirms the number but ran pretty slow.
- Attempt 3 identified an area to increase the speed by 75%.
- Attempt 4 (to do later), will try to optimize the speed further and report more statistics from the experiments.
