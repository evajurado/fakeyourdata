# FAKE YOUR DATA
 
When working with data, one of the problems that can be encountered is the difficulty of accessing real datasets, even internally in a company where, for data protection reasons, information cannot be shared between departments. 

Performing predictive models becomes a complex task when, in many cases, the data has to pass masking processes or even its use is limited to dummy data.

This tool aims to generate fake data based on real data using Deep Learning algorithms using GAN networks. 

This solution allows tabular data to be synthesized so that the variables' distributions of the original dataset remain the same and the relationships between variables is kept. 

Additional use cases might be the improvement of unbalanced or low-quality datasets to be used in Machine Learning models as well as in scenarios where there is no significant volume of training data.

## How To
You can start with the *tabulardatagenerator.ipynb* script by updating the *data_path* field in the first cell or see a working example at *diabetes_tabulardatagenerator.ipynb*. 
For *data_path*, just enter the location of a csv file to be synthesized. 

## Content
The first cell also contains hyperparameters that can be changed to adjust the neural network. 
The code will train the model with your data and generate a dataset named *Unstandarized_Generated_data.csv* in the folder *model*. 
In the notebook, you can visualize the loss function, the network schema and the calculus of the Wasserstein distance to check how accurate is the synthesis. 

## Output
The following images show and example of the comparison between real and fake data analysing regarding their cumulative sums, their distributions and their correlation matrixes.
These visualizations have been generated with TableEvaluator library. 

**Cumulative sums**

![image](https://user-images.githubusercontent.com/11335468/202753288-f4cc0abe-b78e-4d10-9718-dd20c69c4d01.png)

**Variables distributions**

![image](https://user-images.githubusercontent.com/11335468/202753316-f3942b7d-3b25-4369-9312-f0f2a47798fa.png)

**Correlation matrixes**

![image](https://user-images.githubusercontent.com/11335468/202753346-83d2bc23-ee98-44b9-bc9d-0d83da55ca00.png)

## Next steps
Some ideas are:
- Acommodating the tool to sinthesize relational data for data analytics scenarios
- Creating a User Interface to ease its consumption
- Extending data types available including dates, from now on, you can synthesize numeric and categorical values
- Expanding input datasources available, from now on, it is only configured to input csv files 

Collaboration is always welcome !
