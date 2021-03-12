# etl-project

Extract: 2020 DIGIX Advertisement CTR Prediction

-Data was extracted from Kaggle 

-Data was collected by recording advertising patterns, presumably used for machine learning

-Data was de-identified so values in fields in and of themself had little meaning without knowledge of what the values correspond to

Transform:
-To start off the process, we created a new data frame by filtering for only those columns that we wished to include in our database

-Filtered from 37 columns to 17 columns

-We also renamed some of the columns to more accurately describe what we would imagine the data to be

-Because data was masked, we got creative with the database and made our own data 

Load:
-Created 4 parent tables, which were loaded first into the database:
--Careers
--Gender
--Membership
--City Rank

-Followed by main dataset which contained 17 columns

-Loaded into pgAdmin using SQLAlchemy
