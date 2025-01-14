# Pixel-Play-25
# Vision-Language Group (VLG) Recruitment Project
 The project aimed to classify animals based on textual clues and possibly visual data.

## Competition Overview
- **Final Rank:** 30th
- **Public Leaderboard Accuracy:** 57.698% (based on 60% of the test data)
- **Private Leaderboard Accuracy:** 57.035% (based on the remaining 40% of the test data)

- Utilized Resnet, EfficientNet, ConvNeXt models as the backbone for feature extraction and classification.
- Fine-tuned the model on the competition's dataset, optimizing for accuracy on the provided test set.
- Enhanced the training dataset by augmenting images to improve model generalization.
- Also added various other things like Early Stopping, Learning Rate Scheduler,and Optimizer ( Adam,AdamW, SGD) to better the results.
- Divided the training data into Validation data as well to revalidate it after training each epoch.

## Results
- **Best Public Leaderboard Accuracy:** 57.698%
- **Final Private Leaderboard Accuracy:** 57.035%



As per my observation, the main problem was of overfitting, which i tried to tackle via changing the dropout rates, customly defining my own CNN, trying out the best versions of the pretrained models mentioned via experimenting, the validation accuracy on the later codes came out to be much higher than before but still a huge gap from the test accuracy, the increased validation accuracy rate was improving the test accuracy but now by a big margin.

The main challenge of reducing the overfitting and figuring out the ways to better the model test accuracy still remains.
