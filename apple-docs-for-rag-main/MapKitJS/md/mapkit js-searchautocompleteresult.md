

- MapKit JS
-  SearchAutocompleteResult 

Structure

# SearchAutocompleteResult

The result of an autocomplete query, including display lines and a coordinate.

MapKit JS 5.0+

``` source
dictionary SearchAutocompleteResult {
 string[] displayLines;
 mapkit.Coordinate coordinate;
};
```

## Overview

You can use search and search autocomplete in sequence by passing a SearchAutocompleteResult object as the query parameter of a search. For example, you can present the display strings of a collection of search autocomplete results to the user while maintaining a mapping to the original SearchAutocompleteResult object. When the user selects a result, make a search request with the corresponding SearchAutocompleteResult object to retrieve more information about the place.

## Topics

### Autocomplete results

coordinate

The coordinate of the result when it corresponds to a single place.

displayLines

Lines of text to display to the user in an autocomplete menu.

## See Also

### Performing a search autocomplete

autocomplete

Retrieves a list of autocomplete results for the specified search query.

SearchAutocompleteOptions

Options you provide to constrain an autocomplete request.

SearchAutocompleteResponse

An object containing the response from an autocomplete request.

