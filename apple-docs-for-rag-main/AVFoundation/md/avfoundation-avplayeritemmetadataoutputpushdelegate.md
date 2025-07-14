

- AVFoundation
-  AVPlayerItemMetadataOutputPushDelegate 

Protocol

# AVPlayerItemMetadataOutputPushDelegate

Methods you can implement to provide additional metadata.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
protocol AVPlayerItemMetadataOutputPushDelegate : AVPlayerItemOutputPushDelegate
```

## Overview

This protocol extends the AVPlayerItemOutputPushDelegate protocol.

## Topics

### Combining Timed Metadata Groups

func metadataOutput(AVPlayerItemMetadataOutput, didOutputTimedMetadataGroups: [AVTimedMetadataGroup], from: AVPlayerItemTrack?)

Tells the delegate a new collection of metadata items is available.

## Relationships

### Inherits From

- AVPlayerItemOutputPushDelegate
- NSObjectProtocol
- Sendable

## See Also

### Configuring the Delegate

var advanceIntervalForDelegateInvocation: TimeInterval

The time interval, in seconds, the player item metadata output object messages its delegate earlier than normal.

var delegate: (any AVPlayerItemMetadataOutputPushDelegate)?

The delegate object.

var delegateQueue: dispatch_queue_t?

The dispatch queue on which messages are sent to the delegate.

func setDelegate((any AVPlayerItemMetadataOutputPushDelegate)?, queue: dispatch_queue_t?)

Sets the delegate and a dispatch queue on which the delegate is called.

