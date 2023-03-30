# CIS550 Project
Clearly, it took much effort and luck to get nominated for Oscar, the world-top awards, across 1927 to 2023. Currently, we lack a wholesome picture of how these actors and actresses performed in their entire career. Therefore, we will dig into all the works of these outstanding actors and actresses. Combining the Oscar award nominations with Internet Movie Database, IMDB database, we will provide an overview of the movies that they acted in and evaluate their whole career with IMDB ratings from a distinctive perspective. 

Our website will show the list of the nominations for the Oscars. Meanwhile, it allows users to find the other movies that the actor or actress acted in, giving them the chance to find more movies of interest. Besides, users could find their choice of movies based on their personalized criteria, such as comedy movies released in the 1990s. 

## Dataset we used
### Oscar Award, 1927-2023
https://www.kaggle.com/datasets/unanimad/the-oscar-award

The Oscar award data records the Oscar award nominees and winners from 1927 to 2023. 
This data has 10759 rows and 7 columns. The attributes include year of nomination, ceremony number, award category, name, name of film, and winner. Attribute name is the name of the actor, actress, writer, film, or director depending on the award category. 

There are more than 20 awards given each year. However, in this data, there are 134 different award categories, which includes the specific areas of the awards and hence needs to be further cleaned. Also, for the purpose of our website, we decided to only include award categories related to actors and actresses.

Only the attributes name, film, and winner contain missing values. However, the missing values in name and film do not matter because the relevant award categories do not involve actors and actresses. Only the 120 missing values in the winner are problematic, which needs to be deleted from our dataset given the large number of rows in this dataset. 

### IMDB 
https://www.imdb.com/interfaces/

The IMDB contains large amounts of information about movies, TV series, podcasts, streaming, etc. We will be especially interested in the films in this project. This database contains basic information about the film and actors/actresses. Specifically:

(1) title.ratings.tsv contains the ratings of the movies. The ratings dataset has 1282932 rows and 3 columns. The average rating is 6.949, and standard deviation is 1.385. 

(2) name.basics.tsv contains names of 12324725 actors and actresses and their demographic information. 

(3) title.principals.tsv.gz links movies with the actors/actresses acted in it. There are 54780787 linkages and 6 attributes, including one for the movie id and one for the actor/actress id.
