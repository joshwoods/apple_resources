

- AVFoundation
- AVCaptureDevice
-  minimumFocusDistance 

Instance Property

# minimumFocusDistance

The capture device’s minimum focus distance in millimeters.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+

``` source
var minimumFocusDistance: Int { get }
```

## Discussion

For virtual cameras, like builtInDualCamera or builtInTripleCamera, this value represents the smallest minimum focus distance of the autofocus-capable cameras that it sources.

This value is `-1` if the distance is unknown.

