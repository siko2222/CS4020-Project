This project has been utilizing Google Colab.
In this directory you will find:

* The Colab notebook: notebook.ipynb
* Two datasets on csv format
    - overflow_export.csv
    - weather_station_export.csv
* This file, README.txt
* The project report: CS4020ProjectSpring24_<candidate_number>.pdf

How to use the notebook:
1. Upload the notebook to Google Colab
2. Upload the two csv files in the same directory
    - overflow_export.csv and weather_station_export.csv
3. Run the notebook cell by cell (The first cell will install extra libraries)
    - The cells that perform gridsearch for hyperparameter tuning may take very long time, and should not be rerun unless absolutely necessary.

How to use a different optimizer and/or activation function:
1. In the notebook go to 'Model development'->'LSTM'->'Build and train the model'
2. In the cell with # Create the model
    - Change the line dl_model = create_model('SGD', 'tanh', len(X.columns))
    - Alter SGD to another optimizer and or tanh to another activation function
    - If you choose an optimizer that is not imported add this:
        - from keras.optimizers import  <optimizer here>