

- MapKit JS
-  SearchAutocompleteResponse 

Structure

# SearchAutocompleteResponse

An object containing the response from an autocomplete request.

MapKit JS 5.0+

``` source
dictionary SearchAutocompleteResponse {
 string query;
 SearchAutocompleteResult[] results;
};
```

## Topics

### Response

query

The query string used to perform the autocomplete request.

results

The results from an autocomplete request.

## See Also

### Performing a search autocomplete

autocomplete

Retrieves a list of autocomplete results for the specified search query.

SearchAutocompleteOptions

Options you provide to constrain an autocomplete request.

SearchAutocompleteResult

The result of an autocomplete query, including display lines and a coordinate.

