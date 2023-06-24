# Dimensionality Reduction with PCA and Autoencoders

## Introduction
In this project, we explore the techniques of dimensionality reduction using Principal Component Analysis (PCA) and Autoencoders (AE). Dimensionality reduction is a crucial step in data preprocessing, enabling us to extract meaningful information from high-dimensional data while reducing computational complexity. We compare the performance of PCA and AE in terms of reconstruction accuracy, ability to capture complex patterns, and computational efficiency.

## Steps

### 1. Data Overview
- The dataset consists of images with dimensions 360 x 460, which can be considered as a dataset with 360 data points and 460 features/dimensions.
- The goal is to reduce the number of dimensions from 460 to 46, approximately 10% of the original dimensions.

### 2. PCA for Dimensionality Reduction
- PCA is a linear transformation technique that projects data onto orthogonal dimensions that capture maximum variation.
- Calculate the correlation matrix to verify the uncorrelated nature of the transformed features obtained through PCA.
- Reconstruct the original data using the reduced feature space obtained from PCA.
- Measure the Root Mean Squared Error (RMSE) between the original and reconstructed data to assess the reconstruction quality.
- Analyze the gain achieved by PCA in terms of dimensionality reduction and reconstruction accuracy.

### 3. AE for Dimensionality Reduction
- Autoencoders are neural network-based models capable of learning complex relationships and non-linearities.
- Train an AE using gradient descent to minimize the reconstruction loss and reduce the dimensionality of the data.
- Verify the correlation among the transformed features obtained through AE and discuss the impact of training objectives.
- Reconstruct the original data using the reduced feature space obtained from AE.
- Calculate the RMSE between the original and reconstructed data to evaluate the reconstruction performance.
- Analyze the gain achieved by AE compared to PCA in terms of dimensionality reduction and reconstruction accuracy.
- Discuss the impact of AE's flexibility in capturing complex patterns and handling non-linearities.

### 4. Comparing PCA and AE
- Analyze the differences between PCA and AE in terms of their underlying principles, training methods, and performance characteristics.
- Discuss the advantages and disadvantages of each technique based on their ability to capture complex patterns and handle non-linearities.
- Consider the impact of dataset size on the choice between PCA and AE, with a rule of thumb provided for guidance.
- Quantify the gain achieved by AE compared to PCA in terms of dimensionality reduction and reconstruction accuracy.
- Discuss the trade-offs between computational efficiency and performance when using PCA and AE.

### 5. Three-Layer AE with Non-Linear Activation
- Construct a deeper AE architecture with non-linear activation functions to further enhance the model's ability to capture complex patterns.
- Train the three-layer AE and compare its performance with PCA and the previous AE architecture.
- Reconstruct the original data using the reduced feature space obtained from the three-layer AE.
- Calculate the RMSE and quantify the improvement achieved compared to PCA.
- Discuss the impact of the deeper AE architecture and non-linear activations on the model's performance and training time.

## Results
- The RMSE obtained with PCA is 11.84, indicating the reconstruction error when reducing the dimensions to 46.
- The Autoencoder with a single layer and linear activation performs similarly to PCA, with an RMSE of 12.15, which is close to the PCA's RMSE.
- However, the three-layer AE with non-linear activation achieves an RMSE of 8.57, representing a 28% gain over PCA with the same number of reduced dimensions.
- This improvement demonstrates the ability of the deeper AE architecture to capture complex patterns and handle non-linear relationships in the data.

## Conclusion
In conclusion, this project demonstrates the use of PCA and Autoencoders for dimensionality reduction. PCA provides a fast and linear transformation, while Autoencoders offer more flexibility with non-linear activation functions. The results highlight the superior performance of the three-layer AE in capturing complex patterns compared to PCA. However, the choice between PCA and AE depends on factors such as dataset size, complexity of patterns, desired reconstruction accuracy, and available computational resources. The comparison between PCA and AE provides valuable insights for selecting the appropriate technique based on specific requirements.
 
