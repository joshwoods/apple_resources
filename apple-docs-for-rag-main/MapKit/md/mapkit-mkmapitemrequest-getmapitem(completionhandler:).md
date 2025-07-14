

- MapKit
- MKMapItemRequest
-  getMapItem(completionHandler:) 

Instance Method

# getMapItem(completionHandler:)

Requests a map item and calls the provided completion handler.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 15.0+tvOS 18.0+visionOS 1.0+

``` source
func getMapItem(completionHandler: @escaping @MainActor (MKMapItem?, (any Error)?) -> Void)
```

``` source
var mapItem: MKMapItem { get async throws }
```

## Parameters 

`completionHandler`  

A completion handler the framework calls to indicate the success or failure of the map item request.

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can access it as an asynchronous property that has the following declaration:

```
var mapItem: MKMapItem { get async throws }
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Starting and stopping requests

func cancel()

Cancels an in-progress map item request.

