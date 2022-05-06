
# Papkorn - Movie Ratings (MovieLens Approach)

Summary
=======

This dataset (pk-rating-ds) describes like/dislike rating. It contains 26,252 ratings across 5,784 movies. These data were created by 10202 users between October 15, 2021 and May 6, 2022. This dataset was generated on  May 6, 2022.

The data are contained in the files `movies.csv` and `ratings.csv`. More details about the contents and use of all these files follows.

This is a *development* dataset. As such, it may change over time and is not an appropriate dataset for shared research results. 


Content and Use of Files
========================

Formatting and Encoding
-----------------------

The dataset files are written as [comma-separated values](http://en.wikipedia.org/wiki/Comma-separated_values) files with a single header row. Columns that contain commas (`,`) are escaped using double-quotes (`"`). These files are encoded as UTF-8. If accented characters in movie titles or tag values (e.g. Misérables, Les (1995)) display incorrectly, make sure that any program reading the data, such as a text editor, terminal, or script, is configured for UTF-8.


User Ids
--------

Papkorn users ids have been anonymized. User ids are consistent between `ratings.csv` (i.e., the same id refers to the same user across the two files).


Movie Ids
---------

Only movies with at least one rating or tag are included in the dataset. These movie ids are consistent with those used on the IMDB web site. Movie ids are consistent between `ratings.csv` and `movies.csv`.


Ratings Data File Structure (ratings.csv)
-----------------------------------------

All ratings are contained in the file `ratings.csv`. Each line of this file after the header row represents one rating of one movie by one user, and has the following format:

    id,like_movie,user_id,movie_id

The lines within this file are ordered first by user_id, then, within user, by movie_id.

Ratings are made on a like/dislike scale.
1 means that user like the movie and 0 dislikes it.

Movies Data File Structure (movies.csv)
---------------------------------------

Movie information is contained in the file `movies.csv`. Each line of this file after the header row represents one movie, and has the following format:

    id,title,genre,year

Movie titles are entered manually or imported from <https://www.imdb.com/>, and include the year of release in parentheses. Errors and inconsistencies may exist in these titles.

Genres are a pipe-separated list, and are selected from the following:

* Sci-Fi
* Thriller
* Animation
* Comedy
* Family
* Mystery
* Drama
* Crime
* Western
* Fantasy
* Romance
* Horror
* Biography
* History
* War
* Short
* Documentary
* Sport
* Music
* Musical
* News
* Reality-TV
* Film-Noir
* Talk-Show
* Game-Show
* Adult
* Action
* Adventure


Users and Movies
-----------------------

This data collects from <https://t.me/PapkornBot> users from Telegram. Most of users come from Iran and India. So, this dataset contains Persian Movies too.

