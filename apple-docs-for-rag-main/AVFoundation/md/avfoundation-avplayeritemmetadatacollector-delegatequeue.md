

- AVFoundation
- AVPlayerItemMetadataCollector
-  delegateQueue 

Instance Property

# delegateQueue

The dispatch queue on which the delegate’s methods are called.

iOS 9.3+iPadOS 9.3+Mac Catalyst 13.1+macOS 10.11.3+tvOS 9.2+visionOS 1.0+watchOS 2.3+

``` source
var delegateQueue: dispatch_queue_t? { get }
```

## Discussion

This property is not key-value observable.

## See Also

### Accessing the Delegate and Callback Queue

func setDelegate((any AVPlayerItemMetadataCollectorPushDelegate)?, queue: dispatch_queue_t?)

Sets the delegate and a dispatch queue on which the delegate will be called.

var delegate: (any AVPlayerItemMetadataCollectorPushDelegate)?

Accesses the metadata collector’s delegate object.

protocol AVPlayerItemMetadataCollectorPushDelegate

A protocol you implement to receive metadata callbacks from a player item metadata collector.

