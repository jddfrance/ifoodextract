# Ifood API extractor based on latitude and longitude
## Summary 
This is a script to extract data from the Ifood API and derive some maps and graphs from the data obtained. 


This work is still in progress.

## How to use
Simply put the latitude and longitude on the function get_rest like the example (pages is optional, if it's not given it'll just take all restaurants in the area):
![image](https://user-images.githubusercontent.com/95101367/143783521-376ce827-dd57-4ce5-b05f-4271d9e20904.png)

Obs.: Each page has 300 restaurants when searching at max.

## Maps and graphs
### The maps generated:
userRatingCount circle maps
![image](https://user-images.githubusercontent.com/95101367/146431893-cfdb40fc-fe6d-4b4e-8794-c74614d6c9c3.png)

![image](https://user-images.githubusercontent.com/95101367/146432233-a28266fe-2d5a-4527-aa0e-215e59929912.png)

userRatingCount Heatmap

![map](https://user-images.githubusercontent.com/95101367/146432272-00efbce5-d73f-44e3-9f41-3a12fd4120dd.png)

### Barplot generated

![image](https://user-images.githubusercontent.com/95101367/146433477-bbc92ea5-cb75-45e2-936b-bfc6e524bc48.png)


## Some early deductions
From the maps we can see the zones where there's a heavier quantity of user reviews, given by the variable userRatingCount. We can also somehow induce that a higher number of reviews indicates a higher number of revenue and high competition zones are identified in the heatmap with red. An interesting fact is that the biggest restaurant in the city on the Ifood platform is Geek Burger, with around 1800 reviews, which is located on the bottom left part of the map, a zone that has less competition than others. 

Something to note is that, because of the geographic center, some restaurants may be left out of the search, further testing is necessary, but it's still interesting how the comercial center of the capital has less competition than the neighbor city, Ananindeua.

From the bar graph, we can take a look at the distribution of restaraunts vs User Reviews by price range, organized by top reviewed restaurants, at least on a first look there doesn't seem to be a correlation between higher number of reviews and price range, at least determined by price range. Another takeaway we see here is the high number of restaurants on the low end of reviews, which can indicate the hardships the Ifood platform presents to it's commercial users.


## Notes
Because of how many restaurant there are, the script takes some time to find, clean and organize the data, for every 3000 restaurants it finds it takes around 9 minutes to run every execution (measured on Collaboratory).

## Acknowledgments 
The starter point for this project was [this](https://www.kaggle.com/ricardotachinardi/ifood-restaurants-data?select=ifood-restaurants-february-2021.csv) Kaggle post from Ricardo Tachinardi, it was incredibly helpful when searching for methods to access data on Ifood.

