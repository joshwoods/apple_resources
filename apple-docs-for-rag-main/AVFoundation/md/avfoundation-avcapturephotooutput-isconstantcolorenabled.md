

- AVFoundation
- AVCapturePhotoOutput
-  isConstantColorEnabled 

Instance Property

# isConstantColorEnabled

A Boolean value that indicates whether the photo output configures the render pipeline to perform constant color capture.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+

``` source
var isConstantColorEnabled: Bool { get set }
```

## Discussion

The default value is false. Set the value to true to enable support for taking constant color photos. You can only enable constant color capture if the value of isConstantColorSupported is true.

Note

Enabling constant color requires a lengthy reconfiguration of the capture pipeline. If you intend to capture constant color photos, set this property to true before calling startRunning(), or within beginConfiguration() and commitConfiguration() calls on a running capture session.

## See Also

### Configuring Constant Color

var isConstantColorSupported: Bool

A Boolean value that indicates whether a photo output supports constant color capture.

