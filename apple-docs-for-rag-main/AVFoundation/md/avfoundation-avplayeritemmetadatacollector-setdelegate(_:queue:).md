

- AVFoundation
- AVPlayerItemMetadataCollector
-  setDelegate(\_:queue:) 

Instance Method

# setDelegate(\_:queue:)

Sets the delegate and a dispatch queue on which the delegate will be called.

iOS 9.3+iPadOS 9.3+Mac Catalyst 13.1+macOS 10.11.3+tvOS 9.2+visionOS 1.0+watchOS 2.3+

``` source
func setDelegate(
    _ delegate: (any AVPlayerItemMetadataCollectorPushDelegate)?,
    queue delegateQueue: dispatch_queue_t?
)
```

## Parameters 

`delegate`  

An object conforming to AVPlayerItemMetadataCollectorPushDelegate protocol.

`delegateQueue`  

A dispatch queue on which all delegate methods will be called.

## See Also

### Accessing the Delegate and Callback Queue

var delegate: (any AVPlayerItemMetadataCollectorPushDelegate)?

Accesses the metadata collector’s delegate object.

protocol AVPlayerItemMetadataCollectorPushDelegate

A protocol you implement to receive metadata callbacks from a player item metadata collector.

var delegateQueue: dispatch_queue_t?

The dispatch queue on which the delegate’s methods are called.

