
# Ebay used cars dataset

For this exercise, I am going to work on cleaning the data so that it can be easier to use. 
Data was derived from Kaggle: https://www.kaggle.com/orgesleka/used-cars-database/data

### Technologies used
Python

### Data dictionary

|Data type |Meaning|
|----------|-------|
|dateCrawled | When this ad was first crawled. All field-values are taken from this date. |
|name | Name of the car.|
|seller | Whether the seller is private or a dealer.|
|offerType | The type of listing. |
|price | The price on the ad to sell the car.|
|abtest | Whether the listing is included in an A/B test.|
|vehicleType | The vehicle Type. |
|yearOfRegistration | The year in which the car was first registered.|
|gearbox | The transmission type. |
|powerPS | The power of the car in PS. |
|model | The car model name. |
|kilometer | How many kilometers the car has driven. |
|monthOfRegistration | The month in which the car was first registered.|
|fuelType | What type of fuel the car uses.|
|brand | The brand of the car.|
|notRepairedDamage | If the car has a damage which is not yet repaired. |
|dateCreated | The date on which the eBay listing was created.|
|nrOfPictures | The number of pictures in the ad.|
|postalCode | The postal code for the location of the vehicle.|
|lastSeenOnline | When the crawler saw this ad last online. |

#### FYI: 
{These tables were renamed after cleaning the data }

### Steps taken: 
1. Renaming columns
2. Data exploration
3. Update 'price' and 'odometer' type from string to float for easier calculations
4. With the new float values in both columns, using exploration to uncover outliers and excluding them from the dataset
5. Working with dates to unravel data insights (which months had most ads created)
6. Aggregating brand data to display average price and mileage for each of the car brands
7. Recommended next steps

### How to access a summary of the file
1. Go to the files section of the repository and access the 'Ebaycars.ipynb' file by double clicking on it. 
2. Github automatically loads the jupyter notebook file that contains all the comments and findings for the steps mentioned above.

### Next considerations. 

#### Data cleaning next steps:
1. Identify categorical data that uses german words, translate them and map the values to their english counterparts
2. Convert the dates to be uniform numeric data, so "2016-03-21" becomes the integer 20160321.
3. See if there are particular keywords in the name column that you can extract as new columns

#### Analysis next steps:
1. Find the most common brand/model combinations
2. Split the odometer_km into groups, and use aggregation to see if average prices follows any patterns based on the milage.
3. How much cheaper are cars with damage than their non-damaged counterparts?
