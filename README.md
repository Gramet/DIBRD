# DIBRD
DIBRD CrowdAI Blitz May2020
Gaétan Ramet

## Solution

I quickly found that Logistic Regression was working reasonably well on the original data.

Afterwards, I digged into the data a bit more to remove very correlated features and unskew some distributions. I also performed polynomial feature augmentation.

I tried tuning the Logistic Regression as much as possible and also tried to fit other models on the same features, but they were less performant.

Adding Bagging over the Logistic Regression also helped with the robustness. I tried other Ensembling methods (Stacking and Majority voting mostly) with other models but couldn't reach any better than 0.778.