### Achieved
- Designed a multi linear regression model, which is based on the Neural Spikes and Movement of a monkey's hands dataset.
- Also implemented the memoryless linear model.

Different delays were introduced to check the solutions and two approaches were discovered.

- #### Approach 1
  Get the dataset with the for each delayed value adn compute the fitting model till dmax value and find the optimal delay value

- #### Approach 2
  Construct the dataset for the dmax value and make subsets from that set for the required delay value and find the optimal delay value

Empirical Risk (Average Squared Loss) metric is used to compute the optimum delay value

### Conclusion
- When dmax=30, both the approaches only had like 1-2 seconds difference of execution time
- When dmax=60, we can see Approach 1, where Xdly and ydly are generated everytime, it takes 1 min 46 seconds while in Approach 2, where Xdly and ydly for dmax is generated and subsets are taken for the rest of the delay values, in fact its execution time turns out to be 1 min 38 seconds, 8 seconds difference
- As dmax increases, Approach 2 would turn out to be more beneficial in terms of time and space both

~ Aditya Jhaveri
