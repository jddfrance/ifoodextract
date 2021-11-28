# Ifood API extractor based on latitude and longitude
## Summary 
This is a script to extract data from the Ifood API. Instead of downloading locally you can also go [here](https://colab.research.google.com/github/jddfrance/ifoodextract/blob/main/ifood_extract_0.1.ipynb) to execute the script directly.

This work is still in progress.

## How to use
Simply put the latitude and longitude on the function get_rest like the example (pages is optional):
![image](https://user-images.githubusercontent.com/95101367/143783521-376ce827-dd57-4ce5-b05f-4271d9e20904.png)

Obs.: Each page has 300 restaurants when searching at max.

## Notes
Because of how many restaurant there are, the script takes some time to find, clean and organize the data, for every 3000 restaurants it finds it takes around 9 minutes to run every execution (measured on Collaboratory).

## Acknowledgments 
The starter point for this project was [this](https://www.kaggle.com/ricardotachinardi/ifood-restaurants-data?select=ifood-restaurants-february-2021.csv) Kaggle post from Ricardo Tachinardi, it was incredibly helpful when searching for methods to access data on Ifood.

