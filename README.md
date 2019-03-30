# USACO-Gold
Explanations for Gold Problems

Angry
N <= 50,000
Max Radius = 1,000,000,000
Firstly multiply all cow positions by two so everything is always an integer.
Read in the cow positions to a TreeSet (fast ceiling and floor function are very useful).
We have two functions, checkLeft and checkRight, that check if exploding from a given starting point with certain radius can reach all the way left or right respectively. Ceiling and floor are used to check the next haybale affected by an explosion with certain radius and starting from a certain haybale.
Run a binary search on possible radii
  Then, given the radius, binary search for the starting point
  We find the best starting point by testing our radius and start point with checkLeft
  If we reach the left, then move up the lower bound. If we don't, then move down the upper bound.
  After we finish we know we have the greatest point that can still reach left. We then use checkRight, knowing that if isn't
  successful, that radius will never work. If checkRight succeeds, that radius is viable.
Binary search on radius will take Log(Max Radius). Binary search on starting point will also take Log(Max Radius). Checking a starting point will take NLogN. So, overall, it will take (NLogN)(Log(Max Radius)^2)

BalancedPhoto

Censoring

Checklist

Cow248

CowAtLarge

Cownomics

Dream

Feast

FileDirectory

HPS

MooCast

MooTube

PieForPie

Radio

Split

Talent

VisitFarmer
