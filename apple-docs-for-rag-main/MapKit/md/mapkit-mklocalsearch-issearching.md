

- MapKit
- MKLocalSearch
-  isSearching 

Instance Property

# isSearching

A Boolean value that indicates whether the search is in progress.

iOS 6.1+iPadOS 6.1+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
var isSearching: Bool { get }
```

## Discussion

The search object sets the value of this property to true when you initiate a search. It remains in that state until the search object delivers search results (or an appropriate error), at which time the search object sets the value of the property to false.

## See Also

### Performing the search

func start(completionHandler: (MKLocalSearch.Response?, (any Error)?) -> Void)

Starts the search and delivers the results to the specified completion handler.

typealias CompletionHandler

A completion handler block for a search operation.

func cancel()

Cancels an in-progress search operation.

