

- MapKit JS
- PointsOfInterestSearchDelegate
-  searchDidComplete 

Instance Method

# searchDidComplete

Tells the delegate that the search completed.

MapKit JS 5.45+

``` source
void searchDidComplete(
 PointsOfInterestSearchResponse data
);
```

## Parameters 

`data`  

The points of interest fetch results.

## Discussion

MapKit JS calls this method on successful completion of a search request.

## See Also

### Responding to state changes and errors

searchDidError

Tells the delegate that the search failed due to an error.

