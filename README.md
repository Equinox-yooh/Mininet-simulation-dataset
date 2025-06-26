# Mininet-simulation-dataset
Under the Wi-Fi 6 technical architecture, the attenuation characteristics of the signal strength (RSS) value exhibit a nonlinear relationship with the distance between the station and the access point (AP): signal attenuation is significant at close distances, such as when the distance increases from 1 meter to 2 meters, resulting in a sudden drop of 10 dBm in the RSS value; At longer distances, the attenuation rate slows down; for example, from 14 meters to 15 meters, the RSS value decreases by less than 1.5 dBm. Based on this signal propagation characteristic, we constructed two datasets to meet different signal modeling requirements.

## Hyperparameter Selection
|Parameter|Value|
|---|---|
|mode|‘ax’|
|channel|'161'|
|failMode|‘standalone’|
|model|‘logDistance’|
|exp|3.5|
|r0|-25|

## Dataset 1
Contains 88 data points, with RSS values ranging from -25 dBm to -69 dBm. During compilation, we focused on the mapping relationship between signal strength and distance. Based on an in-depth analysis of signal attenuation patterns, we configured a differentiated number of data points in different distance intervals as needed, while avoiding duplicate data collection. This aims to provide precise data support for basic signal modeling based on a limited number of data points. The convergence result of Dataset 1 is 0.19761086.

## Dataset 2
This dataset is more comprehensive, containing 200 data points, with the RSS value range expanded to -25 dBm to -75 dBm. In terms of data organization, an equal number of data points are uniformly distributed across each distance interval, significantly enhancing the overall completeness and randomness of the dataset. Data processing employs a refined strategy, optimizing data quality through flexible adjustment of site locations and introducing two-dimensional transformation techniques to uncover latent data features, thereby providing a more detailed and nuanced data perspective and analytical dimension for signal modeling. The convergence result for Dataset 2 is 0.67944986.
