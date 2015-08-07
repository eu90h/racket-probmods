# racket-probmods
This is some old Racket code I wrote while reading part of the book [Probabilistic Models of Cognition](https://probmods.org/).

The highlight is the rejection-query function, which takes some arbitrary generative model and samples from it according to a 
predicate. The `eval` function made this really easy. 

Unfortunately, rejection-querying is really slow. The Church probabilistic programming language used in the book performs sampling via a Metropolis-Hastings algorithm. Someday I'd like to try implementing a version of Church's `mh-query` procedure.

Since writing this, I learned of two packages for probabilistic programming with Racket:
* [ntoronto's Dr. Bayes](https://github.com/ntoronto/drbayes)
* [rmculpepper's Gamble](https://github.com/rmculpepper/gamble)

So if you're actually trying to do something, you should probably use one of those instead :P
