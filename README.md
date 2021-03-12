# KingsCountyHousing

I began my journey as a practitioner of linear modeling with this project from Flatiron Data Science school. 
I learned that zip codes are essential to building a good model for housing prices. I also used statistics to validate hypothetical features,
which made their way into the model. In addition to zip codes, seasonality and renovation status play into the price. 
That much of the model is interpertable, but much of the model is not.  Since I used polynomial feature engineering there are many variables that are not easily interpretable.  

I had a unique approach to generating new features inspired by genetic heredity. 
I recreated the ordinal directions from a recombination of displacement from an average latitude and longitude point in the data. 
On the face of it, it doesn't make sense.  As my data science teacher observed,  it's not like north and east mated and made a house.
Perhaps some of the other features working together with the artifical ordinal directions, in multidimensional ways, compensated 
for the bizarre, as my root mean square error was within the acceptable range. 

While improving my model, I learned that there is a sweet spot to recursive feature selection. My root mean square error would swing from 
over 2 million to under 200 thousand just because I selected different values for the skips and cv parameters. 

This github repo contains my notebook with the entire modeling process therein, and three csv files: the Kings County Housing Data, the holdout data, 
and Seattle income data. 
