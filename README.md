# Pairs-Trading-Indian-Stocks-using-Machine-Learning
keywords - Kmeans Clustering, Tsne, PCA, Indian Stocks, Johansen test

## FAQs
### What is Pairs Trading?
<b>Ans</b>- It is a trading strategy where we go long on one stock and simultaneously short the other to keep portfolio as much neutral as possible.

### How do you choose stocks in the pair?
<b>Ans</b>- Stocks chosen in the pair should replicate each other’s movement, meaning if one is going up the other should follow and vice-versa, meaning they should possess similarity. Normally, stocks are chosen on the basis of the similarity of their sector, business model, market capitalization, etc.

### How do you find whether stocks are similar? Stocks though in same sector can be dissimilar as well?
<b>Ans</b>- Agreed!

Co-integration test specifies co-movement of price of two stocks and it shows long term relationship between them. There are various ways to test stock’s co-integration. Augmented Dickey Fuller Test, Johansson Test.
Co-integration test the stationarity of the spread between the stocks.

### What is Spread and what is Stationarity?
<b>Ans</b>- Spread is the difference in the price of two stock and stationarity means normalizing the spread.
The normalized spread than hovers around the mean and moves around with some standard deviation.
The idea is to enter a trade by going long in one stock and shorting the other if the spread has deviated a bit from the mean. Once position is been taken we hope the spread to revert back to its mean.

### What if it doesn’t revert to mean and deviates farther apart?
<b>Ans</b>- It may mean the co-integration has broken and that there is a mean shift.

### Hmmm... So it seems choosing appropriate pairs is crucial. How do we go about it?
<b>Ans</b>- 1.	One way is Brute Force. We simply try (n*(n-1))/2 number of combinations and test each combination for co-integration test. This is complex.

2.	Using unsupervised learning.

### Tell me more about unsupervised learning?
<b>Ans</b>- Clustering is one way we can reduce the brute force attempts which adds computing complexity.
K-means clustering algorithm helps in finding similarity between stocks and groups them in clusters using a distance metric called ‘Euclidean Distance’.
This way we can reduce number of co-integration attempts with improved accuracy.

### What is Euclidean Distance?
<b>Ans</b>- Okay enough of talking. Lets dive in the project.

By the way this is Euclidean distance-
https://en.wikipedia.org/wiki/Euclidean_distance





 

