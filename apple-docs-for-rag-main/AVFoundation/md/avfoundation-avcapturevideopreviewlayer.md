

- AVFoundation
-  AVCaptureVideoPreviewLayer 

Class

# AVCaptureVideoPreviewLayer

A Core Animation layer that displays video from a camera device.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+

``` source
class AVCaptureVideoPreviewLayer
```

## Mentioned in 

Setting Up a Capture Session

## Overview

Use this layer to provide a preview of the content the camera captures. A convenient way to use this class in iOS is to set it as the backing layer for a view as shown below.

```
class PreviewView: UIView {
    // Use a capture video preview layer as the view's backing layer.
    override class var layerClass: AnyClass {
        AVCaptureVideoPreviewLayer.self
    }

    var previewLayer: AVCaptureVideoPreviewLayer {
        layer as! AVCaptureVideoPreviewLayer
    }

    // Connect the layer to a capture session.
    var session: AVCaptureSession? {
        get { previewLayer.session }
        set { previewLayer.session = newValue }
    }
}
```

## Topics

### Creating a Preview Layer

init(session: AVCaptureSession)

Creates a layer to preview the visual output of a capture session.

init(sessionWithNoConnection: AVCaptureSession)

Creates a layer to preview the visual output of a capture session, without making connections to eligible video inputs.

### Layer Configuration

var isPreviewing: Bool

A Boolean value that indicates whether the layer is rendering video frames from its source.

var videoGravity: AVLayerVideoGravity

A value that indicates how the layer displays video content within its bounds.

### Session Configuration

var session: AVCaptureSession?

A capture session with visual output to preview.

var connection: AVCaptureConnection?

An object that describes the connection from the layer to a particular input port.

func setSessionWithNoConnection(AVCaptureSession)

Associates a session with the layer without automatically forming a connection to an eligible input port.

### Converting Between Coordinate Spaces

func layerPointConverted(fromCaptureDevicePoint: CGPoint) -> CGPoint

Converts a point from the coordinate space of the capture device to the coordinate space of the layer.

func captureDevicePointConverted(fromLayerPoint: CGPoint) -> CGPoint

Converts a point from layer coordinates to the coordinate space of the capture device.

func layerRectConverted(fromMetadataOutputRect: CGRect) -> CGRect

Converts a rectangle from metadata output coordinates to the coordinate space of the layer.

func metadataOutputRectConverted(fromLayerRect: CGRect) -> CGRect

Converts a rectangle from layer coordinates to the coordinate space of the metadata output.

func transformedMetadataObject(for: AVMetadataObject) -> AVMetadataObject?

Converts a metadata object’s visual properties to layer coordinates.

### Deprecated

Deprecated Symbols

Review unsupported symbols and their replacements.

## Relationships

### Inherits From

- CALayer

### Conforms To

- CAMediaTiming
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Capture preview

class AVCaptureAudioPreviewOutput

A capture output that provides a preview of the captured audio.

