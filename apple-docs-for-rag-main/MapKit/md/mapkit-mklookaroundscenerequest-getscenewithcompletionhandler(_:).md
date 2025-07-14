

- MapKit
- MKLookAroundSceneRequest
-  getSceneWithCompletionHandler(\_:) 

Instance Method

# getSceneWithCompletionHandler(\_:)

Requests a LookAround scene and calls the specified completion handler.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
func getSceneWithCompletionHandler(_ completionHandler: @escaping @MainActor (MKLookAroundScene?, (any Error)?) -> Void)
```

``` source
var scene: MKLookAroundScene? { get async throws }
```

## Parameters 

`completionHandler`  

A completion handler the framework calls when the scene request completes to indicate the success or failure of the request.

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can access it as an asynchronous property that has the following declaration:

```
var scene: MKLookAroundScene? { get async throws }
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Starting and stopping scene requests

func cancel()

Cancels the pending scene request.

