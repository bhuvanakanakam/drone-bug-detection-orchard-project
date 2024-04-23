Drone Based Optimal Bug Detection Algorithm In An Orchard.

### Overview
This project aims to develop a drone-based algorithm for detecting bugs in orchards using aerial imagery. Orchards are vulnerable to various pests and diseases, impacting crop yield and quality. Traditional bug detection methods are often labor-intensive and time-consuming. Leveraging drone technology and computer vision algorithms, we provide an efficient and accurate solution for identifying pests in orchards.

#### Algorithms

An algorithm implemented from the paper, https://www.researchgate.net/publication/359362415_Drone-based_Optimal_and_Heuristic_Orienteering_Algorithms_Towards_Bug_Detection_in_Orchards. And an algorithm of much efficient approach. 

1. Iterate over each aisle in the orchard.
2. For each aisle, sort the rewards of trees in non-decreasing order.
3. Iterate over each possible value of k (from 1 to the number of trees in the aisle).
4. For each value of k, find the largest integer j less than the (budget - 6k)/2 plus 1.
5. Calculate the sum of the top k rewards among trees with indices not exceeding j.
6. Record the top k trees in the set.
7. Calculate the maximum reward for the aisle based on the recorded sets.
8. Repeat steps 1-7 for all aisles.
9. Return the maximum total reward across all aisles.
