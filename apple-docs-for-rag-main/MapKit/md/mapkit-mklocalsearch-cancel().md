

- MapKit
- MKLocalSearch
-  cancel() 

Instance Method

# cancel()

Cancels an in-progress search operation.

iOS 6.1+iPadOS 6.1+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
func cancel()
```

## Discussion

If no search operation is in progress, this method does nothing.

## See Also

### Performing the search

func start(completionHandler: (MKLocalSearch.Response?, (any Error)?) -> Void)

Starts the search and delivers the results to the specified completion handler.

typealias CompletionHandler

A completion handler block for a search operation.

var isSearching: Bool

A Boolean value that indicates whether the search is in progress.

