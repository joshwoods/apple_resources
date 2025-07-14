

- AVFoundation
-  AVCaptureDepthDataOutput 

Class

# AVCaptureDepthDataOutput

A capture output that records scene depth information on compatible camera devices.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
class AVCaptureDepthDataOutput
```

## Overview

This output type captures AVDepthData objects containing per-pixel depth or disparity information, following a streaming delivery model similar to that used by AVCaptureVideoDataOutput. Alternatively, you can capture depth data alongside photos using AVCapturePhotoOutput (see the AVCapturePhotoSettings isDepthDataDeliveryEnabled property).

This object always provides depth data in the format expressed by the source AVCaptureDevice object’s activeDepthDataFormat property. If you wish to receive depth data in another format, choose a new value for that property from those listed in the supportedDepthDataFormats array of the device’s activeFormat object.

## Topics

### Creating a Depth Data Output

init()

Initializes a depth data output object.

### Configuring Depth Data Capture

var alwaysDiscardsLateDepthData: Bool

A Boolean value that determines whether the capture output should discard any depth data that is not processed before the next depth data is captured.

var isFilteringEnabled: Bool

A Boolean value that determines whether the depth data output should filter depth data to smooth out noise and fill invalid values.

### Receiving Captured Depth Data

func setDelegate((any AVCaptureDepthDataOutputDelegate)?, callbackQueue: dispatch_queue_t?)

Designates a delegate object to receive depth data and a dispatch queue for delivering that data.

var delegate: (any AVCaptureDepthDataOutputDelegate)?

A delegate object that receives depth data.

var delegateCallbackQueue: dispatch_queue_t?

A dispatch queue for delivering depth data.

protocol AVCaptureDepthDataOutputDelegate

Methods for receiving depth data produced by a depth capture output.

## Relationships

### Inherits From

- AVCaptureOutput

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Depth data capture

Capturing Photos with Depth

Get a depth map with a photo to create effects like the system camera’s Portrait mode (on compatible devices).

Creating Auxiliary Depth Data Manually

Generate a depth image and attach it to your own image.

Capturing depth using the LiDAR camera

Access the LiDAR camera on supporting devices to capture precise depth data.

AVCamFilter: Applying Filters to a Capture Stream

Render a capture stream with rose-colored filtering and depth effects.

Streaming Depth Data from the TrueDepth Camera

Visualize depth data in 2D and 3D from the TrueDepth camera.

Enhancing Live Video by Leveraging TrueDepth Camera Data

Apply your own background to a live capture feed streamed from the front-facing TrueDepth camera.

class AVDepthData

A container for per-pixel distance or disparity information captured by compatible camera devices.

class AVCameraCalibrationData

Information about the camera characteristics used to capture images and depth data.

