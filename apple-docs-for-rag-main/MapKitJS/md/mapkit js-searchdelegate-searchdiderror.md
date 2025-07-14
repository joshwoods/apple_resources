

- MapKit JS
- SearchDelegate
-  searchDidError 

Instance Method

# searchDidError

Tells the delegate when the search fails due to an error.

MapKit JS 5.0+

``` source
void searchDidError(
 Error error
);
```

## Parameters 

`error`  

The error from a failed search.

## Discussion

MapKit JS calls this method when the search request fails.

## See Also

### Responding to state changes and errors

autocompleteDidComplete

Tells the delegate when the autocomplete request completes.

autocompleteDidError

Tells the delegate when the autocomplete request fails due to an error.

searchDidComplete

Tells the delegate when the search completes.

