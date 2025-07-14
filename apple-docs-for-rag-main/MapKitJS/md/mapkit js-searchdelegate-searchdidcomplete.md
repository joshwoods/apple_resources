

- MapKit JS
- SearchDelegate
-  searchDidComplete 

Instance Method

# searchDidComplete

Tells the delegate when the search completes.

MapKit JS 5.0+

``` source
void searchDidComplete(
 SearchResponse data
);
```

## Parameters 

`data`  

The search results.

## Discussion

MapKit JS calls this method on successful completion of a search request.

## See Also

### Responding to state changes and errors

autocompleteDidComplete

Tells the delegate when the autocomplete request completes.

autocompleteDidError

Tells the delegate when the autocomplete request fails due to an error.

searchDidError

Tells the delegate when the search fails due to an error.

