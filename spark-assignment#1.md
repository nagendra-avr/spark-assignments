### Spark Assignment #1

In this assignment, you will be required to load the movie lens dataset and perform the following transformation.

The movie file contains information about movies in 3 columns. Most of the movies have their debut year added to their names - we want to extract this into separate columns. Genres columns contains multiple categories per row - we want to have them separated into one category per row.

### Program:
##### Write a spark program which performs the following.

1.  Load the movie csv file into Spark RDD.
2.  Split the second column title, to extract the name and year.
3.  Split the third column genres, and append the corresponding genre to the movie along with title and year.
4.  Write the 4 columns separated by comma delimiter to a HDFS location.

### Dataset:

The movie lens dataset can be downloaded [here](https://grouplens.org/datasets/movielens/).

### Input:

`movieId, title,        genres`
`1,Toy Story (1995),Adventure|Animation|Children|Comedy|Fantasy`



### Output:

| movieId  |  title |  year |  genre |
| ------------ | ------------ | ------------ | ------------ |
|  1 | Toy Story  |1995   | Adventure  |
| 1  |  Toy Story |  1995 | Animation  |
|  1 |  Toy Story |  1995 |Children   |
|  1 | Toy Story  |  1995 |  Comedy |
|  1 |  Toy Story |  1995 |   Fantasy|

### Note:
You can perform the above task on any one of the distribution(Hortonworks,Cloudera, AWS EMR or MapR). Submit the program along with output location of HDFS.
