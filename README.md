# PREDICTING A PULSAR STAR:

### WHAT IS A PULSAR STAR?

Pulsar stars are highly magnetized, rapidly spinning neutron stars. A neutron star is formed during an explosion of a star that is at least 8 solar masses, called supernova. As pulsars rotate, their emission beam sweeps across the sky, and when this crosses our line of sight, it produces a detectable pattern of broadband radio emission. As they rotate rapidly, this pattern repeats periodically. Thus, pulsar search involves looking for periodic radio signals with large radio telescopes.


### DATASET AND ATTRIBUTE INFROMATION:

This HTRU2 dataset has different pulsar candidates, collected from the High Time Resolution Universe (HTRU) survey for radio pulsars using Parkes radio telescope. It contains 17,898 candidates, classified into two classes; 1,639 datapoints belonging to positive or class 1 and the rest 16,259 belonging to negative or class 0. Each candidate is described by 8 continuous variables, and a single class variable.

The first four are simple statistics obtained from the integrated pulse profile. This is an array of continuous variables that describe the average emission from a neutron star as a function of its rotational phase, across all the observed time and frequencies. The remaining four variables are similarly obtained from the DM-SNR curve, which shows how the detected signal-to-noise ratio (SNR) varies with dispersion measure (DM). Signal-to-noise ratio describes the strength of the signal compared to random noise and dispersion measure is the integrated column density of free electrons between the observer and the pulsar. The attributes are listed below:

1. Mean of the integrated profile.
2. Standard deviation of the integrated profile.
3. Excess kurtosis of the integrated profile.
4. Skewness of the integrated profile.
5. Mean of the DM-SNR curve.
6. Standard deviation of the DM-SNR curve.
7. Excess kurtosis of the DM-SNR curve.
8. Skewness of the DM-SNR curve.

These are the feature data extracted using the Pulsar Feature Lab tool, which is a collection of python scripts useful for extracting machine learning features from pulsar candidate files.


#### INSTALL:

This project requires Python 3.6 and the following libraries:

* Numpy
* Pandas
* matplotlib
* scikit-learn

It also requires a software installed to run and execute the Jupyter Notebook.


#### OUTPUT (DESIRED TARGET):

* Positive or class 1 (Pulsar star)
* Negative or class 0 (Not a Pulsar star)


#### MODEL TRAINED ON:

By validating using scikit-learn, the accuracy of the following was found to be:

1. Logistic Regression  - 0.9754189944134078
2. K-Nearest Neighbours - 0.9675977653631285

The model is trained on logistic regression for a better accuracy.


#### REFERENCES:

1. R. J. Lyon, B. W. Stappers, S. Cooper, J. M. Brooke, J. D. Knowles, Fifty Years of Pulsar Candidate Selection: From simple filters to a new principled real-time classification approach, Monthly Notices of the Royal Astronomical Society 459 (1), 1104-1123, DOI: 10.1093/mnras/stw656 

2. D. R. Lorimer and M. Kramer, 'Handbook of Pulsar Astronomy', Cambridge University Press, 2005.

3. V. Morello et al., 'SPINN: a straightforward machine learning solution to the pulsar candidate selection problem', Monthly Notices of the Royal Astronomical Society, vol. 443, no. 2, pp. 1651-1662, 2014. 

4. R. J. Lyon, 'PulsarFeatureLab', 2015.

