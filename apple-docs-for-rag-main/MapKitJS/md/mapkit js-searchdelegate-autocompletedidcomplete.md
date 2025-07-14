

- MapKit JS
- SearchDelegate
-  autocompleteDidComplete 

Instance Method

# autocompleteDidComplete

Tells the delegate when the autocomplete request completes.

MapKit JS 5.0+

``` source
void autocompleteDidComplete(
 SearchAutocompleteResponse data
);
```

## Parameters 

`data`  

The results from the search autocomplete request.

## Discussion

MapKit JS calls this method on successful completion of an autocomplete request.

## See Also

### Responding to state changes and errors

autocompleteDidError

Tells the delegate when the autocomplete request fails due to an error.

searchDidComplete

Tells the delegate when the search completes.

searchDidError

Tells the delegate when the search fails due to an error.

