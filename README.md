# Phase 2 Project
This is the repository that contains all files associated with the DS Flex Phase 2 Project.

## Project Overview

In this project, we used exploratory data analysis to investigate trends in film box office sales to genrate market entry insights for a company looking to enter the film industry.

### Business Problem

This company has decided to create a new movie studio, but they don’t know anything about creating movies. Before investing in a large movie project, they need to know which types of movies are doing well, which directors perform well within a reasonable budget, and whihc time of year is best to release. The results of this project are summarized in a preentation suitable to be presented to a non-techinical audience and translated to make clear business recommendations.

### The Data

In the folder `zippedData` are movie datasets from:

* [Box Office Mojo](https://www.boxofficemojo.com/)
* [IMDB](https://www.imdb.com/)
* [Rotten Tomatoes](https://www.rottentomatoes.com/)
* [TheMovieDB](https://www.themoviedb.org/)
* [The Numbers](https://www.the-numbers.com/)

Data from IMDB is located in a SQLite database.

![movie data erd](https://raw.githubusercontent.com/learn-co-curriculum/dsc-phase-2-project-v3/main/movie_data_erd.jpeg)


The data sets used in the investigation were the IMDB SQL database, as well as the The Numbers data set. These data sets were combined to get box office and budget information for specific movies and genres, as well as box office and budget information for specific directors, as well as their ratings. 

Once combined, there were 2,253 entries in the combined movie information and budget data set, and 3,012 entires in the combined director information and budget data set. 

![Alt text](images/Screenshot 2023-09-04 at 11.48.11 AM)
The number of movies relased per year in the combined movie information and budget data set.

![Alt text](images/Screenshot 2023-09-04 at 11.49.03 AM)
The number of movies released per genre in the combined movie information and budget data set. 

### Analysis

The primary analysis work can be found in the jupityer notebook 'data_analysis.ipynb'

Data Cleaning: Movie Information
    - filtered out all movies made before 1980

Data Cleaning:Directors
    - filtered out all directors with less than three movies in the data set 
    - filtered out all directors with average budgets over $100M
    - filtered out all directors with average ratings below 7.0



Data Analysis: 

   - Determine which month is the best time to release a new movie
    
        Most popular month to release: December
        ![Alt text](images/Screenshot 2023-09-04 at 11.58.50 AM)

        Highest grossing months: March, June, November, December
        ![Alt text](images/Screenshot 2023-09-04 at 11.58.44 AM)

        - which genres produce ROI's greater than 1?
        ![Alt text](images/Screenshot 2023-09-04 at 12.01.33 PM)

        - Which Genres are increasing in populatirty?
        ![Alt text](images/Screenshot 2023-09-04 at 12.01.07 PM)

        - Which affordable, experienced directors have the highest ratings and ROI?

        Director Ratings
        ![Alt text](images/Screenshot 2023-09-04 at 12.05.36 PM)

        Director ROI
        ![Alt text](images/Screenshot 2023-09-04 at 12.05.48 PM)
    


### Recommendations

The analysis conlusions are outlined in a non-technical presentation found in this repository under 'Project2_presentation.pptx'

Best months to release: 
    - March 
    - June

Which genres are the best to start out in?
    - most potential: Sci-Fi, Action
    - safest: family, sport, horror

Which directors should we consider?
    - Damien Chazelle
    - Ryan Coogler
    - Christopher Miller & Phil Lord
    - James Wan
