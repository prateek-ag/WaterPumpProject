# WaterPumpProject
DrivenData project (Pump it Up: Data Mining the Water Table)

This is my submission for the competition hosted by DrivenData (https://www.drivendata.org/competitions/7/pump-it-up-data-mining-the-water-table/page/25/).
I have implemented used scikit-learn and keras to implement three different machine learning models for classification:
1) GradientBoost
2) RandomForest
3) NeuralNet

Finally, I have combined the three models into a single ensemble model. To prevent the loss of prediction information from the softmax output of the neural network, I have combined the probabilities from the neural network with the output of the GradientBoost and RandomForest models scaled by 0.8. The scaling factor ensures that the absolute output of GradientBoost and RandomForest models do not dominate over the probabilistic outputs of the NeuralNet model.

Unsurprisingly, validation results indicate that the ensemble method outperforms any individual model. As a result, I make my final predictions using the ensemble model.
