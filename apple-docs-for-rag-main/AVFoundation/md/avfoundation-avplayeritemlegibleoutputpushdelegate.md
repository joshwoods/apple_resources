

- AVFoundation
-  AVPlayerItemLegibleOutputPushDelegate 

Protocol

# AVPlayerItemLegibleOutputPushDelegate

Methods you can implement to provide alternative attributed-string output.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
protocol AVPlayerItemLegibleOutputPushDelegate : AVPlayerItemOutputPushDelegate
```

## Overview

This protocol extends the AVPlayerItemOutputPushDelegate protocol.

## Topics

### Providing Alternative Attributed-String Output

func legibleOutput(AVPlayerItemLegibleOutput, didOutputAttributedStrings: [NSAttributedString], nativeSampleBuffers: [Any], forItemTime: CMTime)

Asks the delegate to process the delivery of new textual samples.

## Relationships

### Inherits From

- AVPlayerItemOutputPushDelegate
- NSObjectProtocol
- Sendable

## See Also

### Configuring the Delegate

var delegate: (any AVPlayerItemLegibleOutputPushDelegate)?

The delegate of the output class.

func setDelegate((any AVPlayerItemLegibleOutputPushDelegate)?, queue: dispatch_queue_t?)

Sets the receiver’s delegate and a dispatch queue on which the delegate is called.

var advanceIntervalForDelegateInvocation: TimeInterval

The time interval, in seconds, that a player item legible output object messages its delegate earlier than normal.

var delegateQueue: dispatch_queue_t?

The dispatch queue on which the delegate is called.

