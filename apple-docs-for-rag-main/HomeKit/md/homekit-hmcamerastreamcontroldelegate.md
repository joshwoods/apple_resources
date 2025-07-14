

- HomeKit
-  HMCameraStreamControlDelegate 

Protocol

# HMCameraStreamControlDelegate

A protocol that gives the delegate updates on the camera stream.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
protocol HMCameraStreamControlDelegate : NSObjectProtocol
```

## Topics

### Observing stream activity

func cameraStreamControlDidStartStream(HMCameraStreamControl)

Tells the delegate that the camera stream has started.

func cameraStreamControl(HMCameraStreamControl, didStopStreamWithError: (any Error)?)

Tells the delegate that the camera stream has stopped.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Observing stream activity

var delegate: (any HMCameraStreamControlDelegate)?

Delegate that receives updates as the camera stream changes.

