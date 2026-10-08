# Assignment 9: Movie Tracker

This program keeps track of which movies each user has watched. It uses a
`HashMap` that maps each user's name to a `HashSet` of the `Movie` objects
they have watched.

## Files

| File | Description |
|------|-------------|
| `Movie.java` | A movie with a title, running time (minutes), release year, and MPAA rating. Overrides `equals`, `hashCode`, and `toString`. |
| `MovieTracker.java` | Stores the movies each user has watched in a `HashMap<String, HashSet<Movie>>`. |
| `Assignment9.java` | Contains `main`. Creates some movies, records who watched them, and prints the results. |

## MovieTracker methods

| Method | Description |
|--------|-------------|
| `addMovie(String userName, Movie movie)` | Records that the user watched the movie. If the user is new, an empty set is created for them first. |
| `getMovies(String userName)` | Returns the set of movies the user has watched. |
| `hasWatched(String userName, Movie movie)` | Returns `true` if the user has watched the movie. |

## Why `Movie` overrides `equals` and `hashCode`

`HashSet` and `HashMap` use `hashCode` to decide where to store an object and
`equals` to decide whether two objects are the same. Two `Movie` objects are
equal when their title, running time, release year, and rating all match.
Equal movies must also have the same hash code, or `contains` will not find
them.

## Compiling and running

From the `Assignment09` folder:

```
javac *.java
java Assignment9
```
