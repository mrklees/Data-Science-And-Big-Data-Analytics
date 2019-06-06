# Recommendation Systems

In this module, we review a few of the most popular algorithms for recommendation systems.

## System 1: Population Averages

The simplest method is to take the average of all available data on a particular item, and then rank them based on that average.

Pros:

* Incredibly easy to implement (no data science required really)

Cons:

* All of them.  If you have no data or little data, either doesn't work or wildly biased from the initial reviews.
* Treats all people as having the same preferences.


### Improvements

There are a few corrections that one can make which address the first con. 

#### Correcting for Small Numbers of Reviews

Take the new rating to be the: $$average rating - Constant/SQRT(# of ratings)$$
