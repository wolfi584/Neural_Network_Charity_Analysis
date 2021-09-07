# Neural_Network_Charity_Analysis

## Analysis Overview
The purpose of the analysis is to develop a binary classifier that will forecast if funded applicants by Alphabet soup will be successful. The project begins by starting with a CSV that has more than 34,000 organizations who have won funding from Alphabet soup in the past. With this information we are to:
- Preprocess the the data
- Compile, train, and evaluate a neural network model
- Submit a report containing results

## Results

### Data Preprocessing
- Target variable(s): Is_Successful, 1
- Feature variable(s): Application_Type, Affiliation_CompanySponsored, Income_Amt, Special_Considerations_N, Special_Considerations_Y
- Removable variable(s): "EIN", and "NAME"


### Compiling, training and evaluating the model
- Selection number of neurons, layers, and activation functions: nodes_layer1 = 100, nodes_layer2 = 30, nodes_layer3 = 10. Two functions are being used - "relu" for the first layers, and "sigmoid" for the remaining layers.
- Explanation for modeling decisions: This particular combination of layers, nodes, and functions produced the best results possible.
- Target model performance: 72.7%
- Attempts to increase model performance: Adjusting the amount of epochs, nodes, and layers. 

## Summary
The most important question to ask post analysis is - is less than 72.7% accuracy acceptable concerning the prediction of successful applicants for Alphabet Soup? If so, this would mean there is a possibility that Alphabet Soup would annualy waste almost 27.3% of their funding on failed projects. If I were Alphabet Soup, I would find 72.7% to be unnacceptable. 

Another import question to ask is - what does the variable 'Is_Successful' truly mean? How does Alphabet Soup categorize a charity as being successful? Are there both quantitave and qualitative measures being used to answer this question? If a charity comes very close to meeting their annual goals but barely misses, would that make them a 'Not_Successful' variable?

My point of asking all these questions is that using a binary model does not allow the answering of all these essential queries. I believe that using a model with multiple linear regressions will allow a more thorough and accurate analysis.



