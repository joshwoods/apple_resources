

- MapKit
- MKLookAroundSnapshotter
-  getSnapshotWithCompletionHandler(\_:) 

Instance Method

# getSnapshotWithCompletionHandler(\_:)

Requests a new snapshot and calls the completion handler you provide.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
func getSnapshotWithCompletionHandler(_ completionHandler: @escaping @MainActor (MKLookAroundSnapshotter.Snapshot?, (any Error)?) -> Void)
```

``` source
var snapshot: MKLookAroundSnapshotter.Snapshot { get async throws }
```

## Parameters 

`completionHandler`  

A completion handler the framework calls to indicate the success or failure of the snapshot request.

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can access it as an asynchronous property that has the following declaration:

```
var snapshot: MKLookAroundSnapshotter.Snapshot { get async throws }
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Starting and stopping a snapshot

func cancel()

Cancels an in-progress snapshot request.

