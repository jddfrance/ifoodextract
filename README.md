# Ifood API extractor based on latitude and longitude

## Summary 
This is a script to extract data from the Ifood API. The starter point for this project was the Kaggle post from Ricardo Tachinardi ([Available here](https://www.kaggle.com/ricardotachinardi/ifood-restaurants-data?select=ifood-restaurants-february-2021.csv)). While it was really helpful, it lacked some things like data on restaurant menus, so I worked on it and found some more information on how to use the API while exploring it. The present script is the result of this work, for non-python users you can just go on the google collab related to the work [here](https://colab.research.google.com/github/jddfrance/ifoodextract/blob/main/ifood_extract_0.1.ipynb) where you can work everything and see the results for yourself.

As a side note, because of how many restaurant there are, the script takes some time to find, clean and organize the data, for every 3000 restaurants it finds it takes around 9 minutes to run every execution (measured on Collaboratory), so for tests it's advisable to run the sub functions or reduce the size variable on the get_ifood function.

This work is still in progress.
