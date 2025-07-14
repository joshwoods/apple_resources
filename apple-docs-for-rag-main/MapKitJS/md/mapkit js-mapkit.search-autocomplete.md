

- MapKit JS
- mapkit.Search
-  autocomplete 

Instance Method

# autocomplete

Retrieves a list of autocomplete results for the specified search query.

MapKit JS 5.0+

``` source
number autocomplete(
 string query,
 function|SearchDelegate callback,
 optional SearchAutoCompleteOptions options
);
```

## Parameters 

`query`  

A string that represents the user’s search in progress.

`callback`  

A callback function or delegate object.

`options`  

With the SearchAutocompleteOptions hash, you have the option to constrain the search to a desired area using the coordinate or region properties. A coordinate or region you supply here overrides the same property you supply to the mapkit.Search constructor. You also have the option to override the language for the search constructor. For example, { `language: ‘fr-CA`’ } tells the server to send results localized to Canadian French. For a complete list of options you can use to constrain your search, see SearchAutocompleteOptions.

## Return Value

This method returns an integer ID that you can pass to the cancel method to cancel a pending request.

## Discussion

To provide the user with a menu of search suggestions, invoke the autocomplete method as users type. This method minimizes typing and brings users the results they’re looking for.

MapKit JS invokes the `callback` function on failure and success with two arguments, `error` and `data`:

- `error`. An error object that contains an error code and descriptive message.

- `data`. A SearchAutocompleteResponse object that the system parses from a server-returned JSON response.

The system doesn’t call the callback function or delegate if you cancel the request before MapKit JS receives a response.

## See Also

### Performing a search autocomplete

SearchAutocompleteOptions

Options you provide to constrain an autocomplete request.

SearchAutocompleteResponse

An object containing the response from an autocomplete request.

SearchAutocompleteResult

The result of an autocomplete query, including display lines and a coordinate.

