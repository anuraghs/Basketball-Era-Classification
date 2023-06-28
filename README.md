# Basketball-Era-Classification
Wrote a Juyptyer Notebook to classify NBA players by era using 2 algorithms: K-Means and Expectation-Maximization (EM) algorithm. Wrote both algorithms from scratch and compared their outpt classifications to the true labels of the dataset

# EM Algorithm
 
Here are the general steps to write an EM algorithm our stats dataset using a Gaussian mixture model:

Initialize the model parameters:
 - The number of mixture components K (in our case 3).
 - The mixing coefficients pi, which are the probabilities of each mixture component. 
 - The means mu and covariances sigma of each mixture component.

E-step: Calculate the responsibilities of each mixture component for each data point. This involves computing the probability density function (PDF) of each mixture component for each data point, and then computing the posterior probabilities of each mixture component using Bayes' theorem and the mixing coefficients.

M-step: Update the model parameters using the responsibilities calculated in E step:

 - Update the mixing coefficients pi using the average responsibilities of each component.
 - Update the means mu of each component using the weighted average of the data points, where the weights are the responsibilities of each component.
 - Update the covariances sigma of each component using the weighted average of the squared distances of the data points from the means, where the weights are the responsibilities of each component.

Repeat steps 2 and 3 until convergence, which is typically defined by a maximum number of iterations or a threshold for the change in the log-likelihood of the data.
