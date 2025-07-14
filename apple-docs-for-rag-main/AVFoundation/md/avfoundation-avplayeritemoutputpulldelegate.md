

- AVFoundation
-  AVPlayerItemOutputPullDelegate 

Protocol

# AVPlayerItemOutputPullDelegate

Methods you can implement to respond to pixel buffer changes.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
protocol AVPlayerItemOutputPullDelegate : NSObjectProtocol, Sendable
```

## Overview

The methods in this protocol are called by AVPlayerItemVideoOutput objects.

## Topics

### Responding to Pixel Buffer Changes

func outputMediaDataWillChange(AVPlayerItemOutput)

Tells the delegate that new samples are about to arrive.

func outputSequenceWasFlushed(AVPlayerItemOutput)

Tells the delegate that a new sample sequence is commencing.

## Relationships

### Inherits From

- NSObjectProtocol
- Sendable

## See Also

### Configuring the Delegate

func setDelegate((any AVPlayerItemOutputPullDelegate)?, queue: dispatch_queue_t?)

Sets the delegate and dispatch queue for the receiver.

var delegate: (any AVPlayerItemOutputPullDelegate)?

The delegate for the video output object.

var delegateQueue: dispatch_queue_t?

The dispatch queue on which to call delegate methods.

