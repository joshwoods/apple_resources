

- MapKit JS
-  PointsOfInterestSearchDelegate 

Class

# PointsOfInterestSearchDelegate

An object or callback function that MapKit JS calls when fetching points of interest.

MapKit JS 5.45+

``` source
interface PointsOfInterestSearchDelegate
```

## Overview

You may pass an object to the search method instead of using of a search delegate callback function. MapKit JS calls the following methods on the delegate object when they exist:

- searchDidComplete – Upon successful completion of a search request, this method returns a data object that is the same as the one passed to the search callback function.

- searchDidError – Called when the search request fails.

## Topics

### Responding to state changes and errors

searchDidComplete

Tells the delegate that the search completed.

searchDidError

Tells the delegate that the search failed due to an error.

## See Also

### Fetching points of interest

search

Fetches points of interest.

PointsOfInterestSearchResponse

The result of a request used to fetch points of interest.

