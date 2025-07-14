

- VisionKit
- DataScannerViewController
-  zoomFactor 

Instance Property

# zoomFactor

The zoom factor for the live video in the camera.

iOS 16.0+iPadOS 16.0+visionOS 1.0+

``` source
@MainActor
var zoomFactor: Double { get set }
```

## Discussion

Set this property to a value between the minZoomFactor and maxZoomFactor properties.

## See Also

### Zooming

var minZoomFactor: Double

The minimum zoom factor that the camera supports.

var maxZoomFactor: Double

The maximum zoom factor that the camera supports.

