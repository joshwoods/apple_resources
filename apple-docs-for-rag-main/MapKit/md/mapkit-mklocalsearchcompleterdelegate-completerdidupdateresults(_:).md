

- MapKit
- MKLocalSearchCompleterDelegate
-  completerDidUpdateResults(\_:) 

Instance Method

# completerDidUpdateResults(\_:)

Tells the method when the specified search completer updates its array of search completions.

iOS 9.3+iPadOS 9.3+Mac Catalyst 13.1+macOS 10.11.4+tvOS 9.2+visionOS 1.0+

``` source
optional func completerDidUpdateResults(_ completer: MKLocalSearchCompleter)
```

## Parameters 

`completer`  

The search completer object with updated results.

## Discussion

After receiving results from a query, the search completer updates its results property with the new MKLocalSearchCompletion objects and calls this method. Use this method to update your app’s interface based on the new search results. For example, you might update a table that you use to display search results to the user.

## See Also

### Getting the search results

func completer(MKLocalSearchCompleter, didFailWithError: any Error)

Tells the method when the specified search completer is unable to generate a list of search results.

