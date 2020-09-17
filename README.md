# Spatio-Temporal-Analysis-on-NYC-Crimes

### 1) How to procede with our code (any additional imports or what to know before/ refer to before going through the project:

* Just open the notebook "NYC_Crimes_Final_Project.ipynb" and import all the files in the beginning and you are good to go.

### 2) What datasets are included, which directory, whats the basic structure of the project, and the direction where we are headed with the project:

* There is data in the "/data" directory that contains all the files imported in our code. There also an excel sheet that has the description of all the variables (Crime_Column_Description.csv). We have changed the names of a few variables in our code though, just for the sake of easy understanding.
* There is some other data in the zipped file that you will see (excel sheets like BRONX_2015, BROOKLYN_2015, etc.). These are the files that were made after we ran a chunk of code in our main file, so they are kept as is.
* "bargraph.mp4" is the video file we have included in our notebook.

### 3) Challenges (experienced or upcoming) with the project's development:

* Even after removing all the NaNs, we had some data that was in float type, for that we had to create a separate function in order to make it work.
* While timestamping the data, in order to mask the data we needed for our analysis, like mentioned before, because of the insignificant data through the years 1015-2012, we faced a problem with using the timestamped data in our EDA, hence we had to use them as strings only for the initial analyses.
* We couldn't figure out why we are getting a wrong confusion matrix even after trying a lot of things and hence we think there is some problem with the data somewhere. We tried Naive Bayes classifier and PCA for our further analysis but we are not sure if the results we are getting are correct or not. This could probably be because we classified the data wrong or our classification is not accurate despite a good precision. The data seems like it is not classified correctly and is varied.

### 4) Limitations:

* We are using NYPD dataset from kaggle website which has the data until the year 2015. They have created this data from NYC open data. NYC open data has NYPD Complaint data history until 2018. As we are using 3 years data, our analysis is limited to a year but it could be improved if we used the whole dataset from NYC open data.
* Also, down our analysis, we figured that the data before 2013 is insignificant to our analysis, probably because of the fact that not many crimes were reported before 2013, so we masked the data we needed. This could influence our analysis, given that we are just using 3 years of data (2013-2015).
