

- MapKit
- MKLocalSearchCompleter
-  results 

Instance Property

# results

The most recently received search completions.

iOS 9.3+iPadOS 9.3+Mac Catalyst 13.1+macOS 10.11.4+tvOS 9.2+visionOS 1.0+

``` source
var results: [MKLocalSearchCompletion] { get }
```

## Discussion

This property is `nil` initially. After a successful query, the search completer sets this property to the array of MKLocalSearchCompletion objects that the query returns. Each new successful query replaces the previous value of this property.

