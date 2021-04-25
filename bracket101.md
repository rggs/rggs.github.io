---
layout: default
---

This was an interesting puzzle, and as a Villanova Wildcat it was right up my alley. I started by trying to figure out
the odds that any one team would advance to round of the "fairly good four". I knew that for each round, the sum of the odds
that any one team would advance past a round would be 1 among all teams that were competing for that spot. For example, the sum
of the odds that the 1, 16, 8, or 9 seeds would make it into the fairly good four should add to one. After some scribbling, it became clear that the 
odds of a team advancing past a round would be:  

$$P_{T,n} = P_{T,n-1}  \sum_{t=j}^k W_{T,t}*P_{t,n-1}$$  

Which can essentially be translated to this: The odds that a team T advances to round n is equal to the sum of the odds of T beating team t,
times the probability that team t advanced past the previous round, where t spans teams j -> k, which are all the teams that can 
possibly advance to that position that T has not already played. That sum is then multiplied by the odds that T advanced past the 
previous round, n-1. So, if we want to know the odds that the 1 seed advances to the fairly good 4 we would do the following:  

* Multiply the odds that the 1 seed beats the 8 seed by the odds that the 8 seed beats the 9 seed.  
* Multiply the odds that the 1 seed beats the 9 seed by the odds that the 9 seed beats the 8 seed.  
* Add these values together.  
* Finally, multiply this number by the odds that the 1 seed beats the 16 seed.  

And there you have it! The code can be found [here](https://github.com/rggs/Jane-Street-Puzzles).
