

- MapKit
- MKMapSnapshotter
-  MKMapSnapshotter.CompletionHandler 

Type Alias

# MKMapSnapshotter.CompletionHandler

A block that processes the results of a snapshot request.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
typealias CompletionHandler = (MKMapSnapshotter.Snapshot?, (any Error)?) -> Void
```

## Parameters 

`snapshot`  

The image data that the snapshotter generates, or `nil` if an error occurs.

`error`  

The error that occurs, or `nil` if the framework generates the snapshot successfully.

## See Also

### Generating a snapshot

func start(completionHandler: (MKMapSnapshotter.Snapshot?, (any Error)?) -> Void)

Submits the request to create a snapshot and delivers the results to the specified block.

func start(with: dispatch_queue_t, completionHandler: MKMapSnapshotter.CompletionHandler)

Submits the request to create a snapshot and executes the resulting block on the specified queue.

func cancel()

Cancels the request to create a snapshot.

var isLoading: Bool

A Boolean value that indicates whether the snapshotter is generating an image.

