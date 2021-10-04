# Tanzanian-water-point-classification

This projects objective is to see if we can create a model that can classify Tanzanian water points correctly with a threshold of 60%.

To see the results from this analysis run the "water point classification file" in main folder



we say that the best performing model was random forest,  with a 4 cross validated test score of 82%, best parameters

criterion=entropy​

n_estimators=500​

min_samples_split=5

We can also see that the best metrics from our analysis at determining if the wells were good are

![alt test](https://github.com/criolloprimero/Tanzanian-water-point-classification/blob/main/graphs/top%20selectors.PNG)

-GPS height
-is their enough water, quantity
-the year built
-population size
-amount of water to be pulled

From this we can recommend some suggestion to what to look for:

1.We can see that the amount of water available to pull has a drastic affect,
We can say that any point with points above 50000 would be a good point.

![2nd graph](https://github.com/criolloprimero/Tanzanian-water-point-classification/blob/main/graphs/amount%20tsh.PNG)


2. we can also see that the more recently built water wells were far more likely to be functional. than those built before 1985

![3rd graph](https://github.com/criolloprimero/Tanzanian-water-point-classification/blob/main/graphs/construction%20year.PNG)


3. when we take a look at the gps height, it gets a little bit trickier when taking a look at the binned height and intervals you notice that those water wells that were above average for any of the heights within a range of 10 it was more likely to be functional. I am not sure how to rationalize this one other than as we saw in the first point the more water available would make the well more prone to repair. which would be at lower altitudes as water pools into rivers and lake.

![3rd graph](https://github.com/criolloprimero/Tanzanian-water-point-classification/blob/main/graphs/gps%20height.PNG)

4. another point is if there is enough water available, it is disproportionately going to be functioning/

![4th graph](https://github.com/criolloprimero/Tanzanian-water-point-classification/blob/main/graphs/quantity%20enough.PNG)
