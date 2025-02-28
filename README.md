# Machine-Learning
Practice in ML

Some notes and the results of supervised learning VS unsupervised learning
1. In short, if labels are available, use CNN;
If no labels are available, use PCA + K-means.
2. CNN outperforms PCA + k-means in classification accuracy.
Unsupervised clustering works well for exploratory analysis but does not generalize well for 
CIFAR-100.
PCA + k-means can be used as a preprocessing step to improve CNN training efficiency.

3.Comparison table for using CIFAR-100

Feature                Supervised (CNN)               Unsupervised (PCA + K-Means)

Requires Labels?            Yes                                     No
Accuracy                   50-70%                        ~30-40% (Cluster Purity)
Computational Cost     igh (GPU needed)                   Low (runs fast on CPU)
Feature Learning     Learns deep features             Relies on raw pixel intensities
Overfitting Risk     Yes (if not regularized)             No(no labeled training)
Scalability          High (with deep models)           High (for exploratory analysis
