# Data Science Phase 1 Project
This project Required us to create concrete suggestions to microsoft studios in order for them to create a succesful film.
My suggestions revolve around the studio they decide to film with in order to make their movie.
Production studios make up a significant amount of the production budget so I want to create a metric based off the data available that would identify successful  studios.
In order to create this metric I merged two data frames on each other. 
After cleaning both data frames they were merged on a common column 'Movie' that was a column containg movie names. This new data frame was able to show studio data combined with production and worldwide gross data.

## ROI by studio
To create this metric I made a new column in the dataframe I recently merged and assigned the value to the studios net worldwide gross over the studios net production budget. This gave me a float value signifying the factor that when multipled by a production budget returned the average worldwide gross. For example if the ROI was 4.0 and the production budget is $1,000,000 you can expect a worldwide gross of about $4,000,000 from this studio.
![ROI](/images/roi.png)

## Analyzing ROI
I wanted to be able to suggest an average budget microsoft studio should expect to start with. To do this I narrowed down my studio suggestions to Universal and Fox. I chose these two studios because they had high ROI's and a great number of movies produced. The number of movies produced is significant because it acts as a studio's sample size, the greater the sample size the more accurate the approximation metric of ROI will be. Studios with higher movie counts hypothetically have ROI values that more accurately approximate their actual value.
![mc_by_studio_top_ten](/images/mc_by_studio_top_ten.png)

## Calculating Budget
This was a straight forward step which I calculated both Fox and Universal's average production budget based on the 110 movies produced by Fox Studio and the 117 movies produced by Universal Studio.