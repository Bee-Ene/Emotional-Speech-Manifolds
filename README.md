# Emotional-Speech-Manifolds
Analysis of Emotional Speech Manifolds using Feature Learning, t-SNE and Spectral Clustering

This project investigates whether emotional speech signals contain an underlying nonlinear geometric structure that can be discovered through manifold learning techniques.
Speech emotion recognition is a challenging high-dimensional problem as acoustic features extracted from speech are often not linearly separable. The aim of the work was to analyze the intrinsic structure of emotional speech representations and determine whether nonlinear dimensionality reduction and graph-based clustering methods can reveal meaningful emotion groupings.
I used the RAVDESS emotional speech dataset. It consists of 2880 speech recordings from 24 actors across 8 emotion categories: neutral, calm, happy, sad, angry, fearful, disgust, and surprised.
Mel-Frequency Cepstral Coefficients (MFCCs), Chroma features and Spectral contrast features were used for transforming the audio signals to feature vectors, producing a 99-dimensional acoustic representation for each audio sample. After which the extracted features were standardized and analyzed using Principal Component Analysis (PCA), t-SNE and Spectral Clustering.
PCA showed limited emotion separation, suggesting that linear methods are not sufficient enough to capture the complexity of emotional speech. For t-SNE, it revealed clearer local structures and grouping patterns, suggesting that emotional speech likely lies on a nonlinear manifold. While spectral clustering was applied using a nearest-neighbor affinity graph to analyze connectivity-based emotion organization.

PCA: Weak linear separation
t-SNE: Clear local grouping
Spectral clustering: Graph-based emotion structure 

Insight:
Emotional speech is not linearly separable
Strong overlap exists between similar emotions

Finally, the results suggest that manifold learning methods provide better insight into the hidden structure of emotional speech as compared to linear approaches. 

Future improvements could involve more advanced embeddings, better evaluation methods for the clustering, and supervised classification models built on manifold representations.
