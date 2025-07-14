

- MapKit
- MKMapSnapshotter
-  cancel() 

Instance Method

# cancel()

Cancels the request to create a snapshot.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
func cancel()
```

## Discussion

If the snapshotter isn’t in the process of generating the snapshot, calling this method does nothing.

## See Also

### Generating a snapshot

func start(completionHandler: (MKMapSnapshotter.Snapshot?, (any Error)?) -> Void)

Submits the request to create a snapshot and delivers the results to the specified block.

func start(with: dispatch_queue_t, completionHandler: MKMapSnapshotter.CompletionHandler)

Submits the request to create a snapshot and executes the resulting block on the specified queue.

typealias CompletionHandler

A block that processes the results of a snapshot request.

var isLoading: Bool

A Boolean value that indicates whether the snapshotter is generating an image.

