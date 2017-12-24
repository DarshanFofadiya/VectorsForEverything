# VectorsForEverything

The concept of creating vectors for entities is a very powerful one, and helps encode information in a dense format.
In general, while building machine learning models, we tend to skip the information contained in the identifier column.
However, if we could train a neural network to create vectors for every identifier such that the vectors learn very crucial information,
otherwise missing in the data, it can create wonders

The create_embeddings.py contains a fucntion called calcVectors which helps you do this exactly for your data.

Steps to use the function:

	Load your data
	Do the necessary cleaning and pre processing
	Convert the data type of all the columns for which vectors have to be created to "category"
	Call the function calcVectors with 2 arguments: Data object passed as a pandas Dataframe and the name of the y variable as string
	You will get the output of all the categorical variables as vectors
