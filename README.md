# MiguelSaraiva-ALLClassifier
A VGG16 model that analysis cell extraction images and determines wether a patient is suffering from Acute Lymphoblastic Leukemia.

Initially, due to imbalanced data, the model was not performing as expected, showing the following metrics:

Accuracy:0.9062
Loss:0.6892
Precision:0.8431372549019608
Recall:0.8396911898274296

With these numbers, we could see roughly 1 in 6 patients would be given either a false positive or a false negative diagnosis.

Upon artificially increasing the smaller data class (Benign examples) by duplicating the existing images and applying a random rotation, the data became more balanced and the model was able to achieve the following metrics:

Accuracy:0.9375
Loss:0.6451
Precision:0.8464106844741235
Recall:0.9218181818181819

With these numbers, we can see roughly 1 in 6 patients would be given a false positive diagnosis where roughly 1 in 11 patients would be given a false negative diagnosis.
