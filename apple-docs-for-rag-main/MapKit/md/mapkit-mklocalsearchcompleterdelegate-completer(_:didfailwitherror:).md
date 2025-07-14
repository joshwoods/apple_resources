

- MapKit
- MKLocalSearchCompleterDelegate
-  completer(\_:didFailWithError:) 

Instance Method

# completer(\_:didFailWithError:)

Tells the method when the specified search completer is unable to generate a list of search results.

iOS 9.3+iPadOS 9.3+Mac Catalyst 13.1+macOS 10.11.4+tvOS 9.2+visionOS 1.0+

``` source
optional func completer(
    _ completer: MKLocalSearchCompleter,
    didFailWithError error: any Error
)
```

## Parameters 

`completer`  

The search completer object reporting the error.

`error`  

The error object containing the reason for the failure.

## Discussion

Use this object to process any errors that occur while generating search results. Even when an error occurs, the search completer starts a new search if it already has a new search string. Depending on the error, you might do nothing or let the user know that you were unable to obtain a list of search completions.

## See Also

### Getting the search results

func completerDidUpdateResults(MKLocalSearchCompleter)

Tells the method when the specified search completer updates its array of search completions.

