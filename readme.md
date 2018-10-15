## Project: Classification of Political Party Affiliation

Using data compiled by the American National Election Studies (ANES) organization, I attempt to predict the political party preference of an individual based purely on demographic information.  To do so, I extracted features I deemed important through the exhaustive list of nearly 1,300 features and use these features as inputs into a supervised classification algorithmic pipeline. My output, party preference, is also a column in the ANES dataset, and I used this as my target variable.  I looked into two subsets of the data: one, a historical set that include survey data from 1952-1960, and the other a modern dataset that includes survey data from 2004-2012. 


### Install

This project requires **Python 2.7** and the following Python libraries installed:

- [NumPy](http://www.numpy.org/)
- [Pandas](http://pandas.pydata.org)
- [matplotlib](http://matplotlib.org/)
- [scikit-learn](http://scikit-learn.org/stable/)

You will also need to have software installed to run and execute an [iPython Notebook](http://ipython.org/notebook.html)


### Files

`modern.ipynb` --> Python notebook where the code is implemented for the modern dataset.

`historical.ipynb` --> Python notebook where the code is implemented for the historical daraset.

`visuals.py` --> visualization functionality produced by Udacity

`project.pdf` --> The detailed report of the project's findings. 




### Run

In a terminal or command window, navigate to the top-level project directory `finding_donors/` (that contains this README) and run one of the following commands:

```bash
ipython notebook finding_donors.ipynb
```  
or
```bash
jupyter notebook finding_donors.ipynb
```

This will open the iPython Notebook software and project file in your browser.

### Data

The ANES data can be found at the following link: 

http://www.electionstudies.org/studypages/download/datacenter_all_NoData.php

It is called the "ANES Time Series Cumulative Data File" and you will need to sign up for a free account in order to access the data.  I used the stata file since it can easily be imported into Python using Pandas.  

**Important Features**
- `reviews`: the number of reviews the host as received. 
- `ratings`: the rating of the host on a five-point scale. 
- `private_room`: if the listing offers a private room.
- `entire_place`: if the listing offers the entire listing.  
- `plus`: whether or not the host is considered a "plus" host.  
- `rental_price_norm`: an engineered feature that includes the median rental price for each district. 
- `shared_room`: if the listing offers a shared room.
- `number_of_beds`: the number of beds the listing offers. 
- `number_of_guests`: the number of guests the host can offer. 

There are several more features that as pertinent not listed here. 

**Target Variable**
- `price` the price that the host the Airbnb should set their listing to.

