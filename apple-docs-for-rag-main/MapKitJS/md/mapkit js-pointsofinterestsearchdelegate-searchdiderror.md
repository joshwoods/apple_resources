

- MapKit JS
- PointsOfInterestSearchDelegate
-  searchDidError 

Instance Method

# searchDidError

Tells the delegate that the search failed due to an error.

MapKit JS 5.45+

``` source
void searchDidError(
 Error error
);
```

## Parameters 

`error`  

The error from a failed fetch for points of interest.

## Discussion

MapKit JS calls this method when the search request fails.

## See Also

### Responding to state changes and errors

searchDidComplete

Tells the delegate that the search completed.

