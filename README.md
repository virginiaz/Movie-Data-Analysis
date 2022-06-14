# Movie-Data-Analysis
Film-making business is a risky investment and the purpose of this analysis is to analyze the variables involved and should be implemented in order to be lucratively profitable in the movie studio business .

## WHAT TOOLS DO I NEED?
To complete this analysis, the following software requirements will be used: 
<li> Python 3
<li> NumPy
<li> Pandas -  package for data manipulation and analysis in Python.
<li> SQLite3
<li> PandaSQL
<li> Matplotlib
<li> Seaborn
<li> Jupyter Notebook
<li> Anaconda   
    
  ##  THE FILES
  
  There are six movie dataset files. All six of these files are zipped up. To access these six data files, they need to be unzipped using Python individually.
<ol type=1>
<li>boxoffice.csv.gz
<li>rottentomatoes.tsv.gz
<li>rottentomatoes.reviews.tsv.gz
<li>themoviedatabase.csv.gz
<li>thenumbers.csv.gz"
<li> im.db.zip 
</ol>

  In this analysis, randomly selected data for the movies released date years between 1930 through 2022 are provided.  I will be analyzing over 4  million records of raw data (4,463,522 records from all data files) provided by Box Office Mojo, Rotten Tomatoes, The Movie Database,The Numbers and the IMDB.


The __Box Office Mojo__ csv file contains _five (5)_ columns:

- 'title' (e.g., Toy Story 3)
- 'studio'(e.g., BV)
- 'domestic_gross'(e.g., 415000000)
- 'foreign_gross'($ e.g., 652000000)
- 'year'(e.g., 2010)


The __Rotten Tomatoes__ tsv file contains _twelve (12)_ columns:

- 'id'(e.g.,1890)
- 'synopsis'(e.g.,A misplaced sausage and his savory friends)
- 'rating'(e.g.,R)
- 'genre'(e.g., Comedy)
- 'director'(e.g.,Conrad Vernon)
- 'writer'(e.g., Seth Rogen)
- 'theater_date'(e.g., Aug 12, 2016)
- 'dvd_date'(e.g., Nov 8, 2016)
- 'currency'(e.g., $)
- 'box_office'(e.g., 97,661,826)
- 'runtime'(e.g., 89 minutes)
- 'studio'(e.g., Sony Pictures)
       

The __Rotten Tomatoes__ Reviews tsv file contains _eight (8)_ columns:
- 'id'(e.g.,3)
- 'review'(e.g.,For one of the smartest films I've seen)
- 'rating'(e.g.,4/5)
- 'fresh'(fresh or rotten)
- 'critic'(e.g.,Patrick Kolan)
- 'top_critic'(0 or 1)
- 'publisher'(e.g.,Shotgun Cinema)
- 'date'(e.g.,September 26, 2012)
       
   
The  __Movie Database__ csv file contains _nine (9)_ columns:
- 'genre_ids'(e.g.,12)
-'id'(e.g.,299536)
- 'original_language'(e.g.,en)
- original_title'(e.g.,Avengers: Infinity War)
- 'popularity'(e.g.,80.773)
- 'release_date'(e.g.,2018-04-27) 
- 'title'(e.g.,Avengers: Infinity War)
- 'vote_average'(e.g.,8.3)
- 'vote_count'(e.g.,13948)


The __Numbers__ csv file contains _six (6)_ columns:
- 'id' (e.g.,1)
- 'release_date' (e.g.,Dec 18, 2009)
- 'movie'(e.g.,Avatar)
- 'production_budget' (in dollars, e.g., 425,000,000)
- 'domestic_gross' (in dollars, e.g.,760,507,625)
- 'worldwide_gross' (in dollars, e.g, 2,776,345,279)

      
The __IMDB__ zip file contains _eight(8)_ tables:
- directors      
- movie_akas
- movie_ratings
- principals   
- known_for
- movie_basics
- persons
- writers    


> The __movie_basics__ table has _six (6)_ columns:  
> * movie_id (e.g.,tt0069049)
> * primary_title (e.g.,The Other Side of the Wind)
> * original_title(e.g.The Other Side of the Wind)
> * start_year(e.g.,2018)
> * runtime_minutes(e.g.,122.0)
> * genres(e.g.,Drama)

> The __movie_ratings__ table has _three (3)_ columns:  
> * movie_id (e.g.,tt10356526)
> * averagerating(e.g.,8.3)
> * numvotes(e.g.,31)
 
>The __imdb_movie_akas__ table has _eight (8)_ columns:    
> * movie_id (e.g.,tt0369610)
> * ordering (e.g.,14)
> * title (e.g.,Jurassic World)
>* region(e.g.,FR)
>* language (e.g.,en)
>* types (e.g.,imdbDisplay)
>* attributes (e.g.,short title	)
>* is_original_title (e.g.,1.0)


> The __imdb_known_for__ table has _two (2)_ columns:  
> * person_id (e.g.,nm0061671)
> * movie_id  (e.g.,tt0837562)
       
> The __imdb_principals__ table has _six (6)_ columns:  
> * movie_id (e.g.,tt0111414)
> * ordering (e.g.,1)
> * person_id (e.g.,nm0246005)
> * category (e.g.,actor)
> * job  (e.g.,producer)
> * characters (e.g.,The Man)
    
> The __imdb_writers__ table has _two (2)_ columns:  
> * movie_id (e.g.,tt0285252)
> * person_id (e.g.,nm0899854)
    
> The __imdb_directors__ table has _two (2)_ columns:  
> * movie_id (e.g.,tt0878654)
> * person_id (e.g.,nm0089502)

> The __imdb_persons__ table has _five (5)_ columns:  
> * person_id  (e.g.,nm9990381)
> * primary_name (e.g.,Susan Grobes)
> * birth_year (e.g.,)
> * death_year (e.g.,)
> * primary_profession  (e.g.,actress)
