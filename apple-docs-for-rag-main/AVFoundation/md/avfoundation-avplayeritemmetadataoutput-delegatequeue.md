

- AVFoundation
- AVPlayerItemMetadataOutput
-  delegateQueue 

Instance Property

# delegateQueue

The dispatch queue on which messages are sent to the delegate.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
var delegateQueue: dispatch_queue_t? { get }
```

## See Also

### Configuring the Delegate

var advanceIntervalForDelegateInvocation: TimeInterval

The time interval, in seconds, the player item metadata output object messages its delegate earlier than normal.

var delegate: (any AVPlayerItemMetadataOutputPushDelegate)?

The delegate object.

protocol AVPlayerItemMetadataOutputPushDelegate

Methods you can implement to provide additional metadata.

func setDelegate((any AVPlayerItemMetadataOutputPushDelegate)?, queue: dispatch_queue_t?)

Sets the delegate and a dispatch queue on which the delegate is called.

