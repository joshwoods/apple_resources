

- MapKit JS
- SearchDelegate
-  autocompleteDidError 

Instance Method

# autocompleteDidError

Tells the delegate when the autocomplete request fails due to an error.

MapKit JS 5.0+

``` source
void autocompleteDidError(
 Error error
);
```

## Parameters 

`error`  

The error from a failed autocomplete request.

## Discussion

MapKit JS calls this method when an autocomplete request fails.

## See Also

### Responding to state changes and errors

autocompleteDidComplete

Tells the delegate when the autocomplete request completes.

searchDidComplete

Tells the delegate when the search completes.

searchDidError

Tells the delegate when the search fails due to an error.

