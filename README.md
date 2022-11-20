# Exploring the impact of the number of tournaments and crossover probability on the fitness of Full Microbial Genetic Algorithms.

We investigate the change in performance of a Full Microbial Genetic Algorithm (FMGA) with variations in the number of tournaments and crossover rate.

The first two parts investigate the hyper-parameters individually, and the final one aims to find the optimal number of each.

In the first part, we generate multiple FMGAs, run them over 10’000 tournaments, and make an average of their best fitness at each tournament to plot its progress.
<img width="1284" alt="Screenshot 2022-11-20 at 00 48 59" src="https://user-images.githubusercontent.com/56508673/202877536-2c4ed1ff-eff5-4d24-b451-f73d2fdf99cb.png">

In the second part, we follow the same method but create averaged subsets of FMGAs where each group has a different crossover rate, and investigate the assumptions of this parameter. We found it relies heavily on the initial diversity of the population.
<img width="1130" alt="Screenshot 2022-11-20 at 00 49 32" src="https://user-images.githubusercontent.com/56508673/202877548-82c6a5c9-6074-4c05-b35a-bca37abdea04.png">

In the third part, we create a heat-map of many subsets of FMGAs with varying numbers of tournaments and crossover rates to show which combination performs best.
<img width="1114" alt="Screenshot 2022-11-20 at 00 50 22" src="https://user-images.githubusercontent.com/56508673/202877558-a04948e5-1e38-4639-a458-d2083b4b9527.png">

We measure the performance by making our FMGAs solve the knapsack problem. We found that the crossover rate had much less impact than the number of tournaments on the fitness of an FMGA, as long as it is between 0.2 and 0.9.
