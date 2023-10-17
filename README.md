# Data-Wrangling
Getting dataset from twitter, more specifically WeRateDogs twitter data, then clean to create interesting analysis

Data Gathering:
The project involved gathering three datasets: a csv file, a tsv file and a JSON file.
1st Dataset
The first csv file, “twitter-archive-enhanced.csv” was provided on Udacity classroom. The csv file was downloaded manually and read into python using pandas. The dataset had 2356 rows and 17 columns.
2nd Dataset
The second file, “image-predictions.tsv”, was from a url. It was read into python using the request library. I had to create a new file and write into the file and saved as tsv file. The dataset has 2075 rows and 7 columns
3rd Dataset
The third data was supposed to be accessed and downloaded using twitter’s API. It required access from twitter developmental team. I requested access from the team, I had to fill several forms on the purpose and nature of the analysis.
Unfortunately, I didn’t get the access key or token, so I defaulted to manually downloading the JSON file(txt) from Udacity and extracting columns of interest from the dictionary. Data was extracted using a for loop, where I iterated over every line in the txt, collecting tweet id, retweet count, favorite count and followers count. All four columns were extracted into a dictionary called df_list. I subsequently converted df_list to a dataframe for exploration and data analysis.
Data Cleaning:
I identified some quality and tidiness issues with the dataset.
