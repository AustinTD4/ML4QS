This repository stores code, data, and a report for a school project. The course was Machine Learning for the Quantified Self. The project was to create machine learning algorithms that could recognize the activity the phone user (between sitting, walking, running, and cycling) and predict current cadence (steps mer min or revolutions per min) based on a ten second window of accelerometer and gyroscope data. A partner and I gathered accelerometer and gyroscope data from our phones while conducting a series of movement experiments, generating a few hours total of data. This data was labeled by hand in order to faciliate a supervised learning environment. We thought of this project ourselves, had supervision from a student advisor, and all the code in this repository represents our original work. The project was completed in the span of four weeks. 

Principal component analysis was used to reduce the complexity of the data from its 9 original inputs. The data was filtered and transformed using the Kalman filter and Fourier transformations, while statistical matrics about the distribution of observations were added to the raw data. Machine learning algorithms were applied to windows of observations in the dataset, using both dense and sparse representations. The dense representation retained all available features from the observations, giving a comprehensive view of the data. In contrast, the sparse representation focused on a subset of the most significant features, removing redundant or less informative ones. 

Deep Neural Networks, LSTMs, TCNs, and Random Forests were applied to the tasks of classification (for activity) and regression (for cadence). The best results are discussed in detail at the conclusion to the report (ML4QS_Report) included in this repository.

FOLDERS:
[Data Samples] -- Contains true original data gatered from experimenters measured at 20Hz.
[Filtered Data] -- Contains original and PCA transformed data after using the Kalman filter to remove noise and outliers.
[Final Data] -- Contains the data used to train the machine learning algorithms.
[Fourier] -- Contains visualizations for the Fourier transformations of each input from each activity sample.

### FOLDERS:
- **Data Samples**: Contains true original data gathered from experimenters measured at 20Hz.
- **Filtered Data**: Contains original and PCA transformed data after using the Kalman filter to remove noise and outliers.
- **Final Data**: Contains the data used to train the machine learning algorithms.
- **Fourier**: Contains visualizations for the Fourier transformations of each input from each activity sample.
