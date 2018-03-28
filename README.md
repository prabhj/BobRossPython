#### (NOTE : Please click on the databricks link given on top of this page to access the project.)

# Clustering Bob Ross' Paintings using K-means

## Background
Bob Ross
For this I have used k-means clustering to analyse Bob Ross paintings. I was inspired by the FiveThirtyEight article on his work, which you can read for background: https://fivethirtyeight.com/features/a-statistical-analysis-of-the-work-of-bob-ross/
For those of you unfamiliar with Bob ("Happy Trees") Ross... check out his videos on YouTube (e.g. https://www.youtube.com/watch?v=kJFB6rH3z2A) and the Wikipedia page on him. Along with the data provided by fivethirtyeight I  also augmented it with the actual images. I've downloaded a few hundred thumbnails and will use those as well.

## Getting the data from Amazon Web Services S3
We need the CSV file with data (bob_ross.csv), as well as a collection of images to complete this assignment. One way for us to share those with you is to put them in an AWS S3 bucket and get you to "mount" that bucket as a directory that's accessible via this notebook.

To Spark, it will look like the files live in a directory called /mnt/si330w18.
To pandas, which we will use to read the data, the files will live in /dbfs/mnt/si330w18. Note the use of /dbfs as a prefix in the pandas version.
