

- WebKit
- WKSnapshotConfiguration
-  snapshotWidth 

Instance Property

# snapshotWidth

The width of the captured image, in points.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+

``` source
@NSCopying @MainActor
var snapshotWidth: NSNumber? { get set }
```

## Discussion

Use this property to scale the generated image to the specified width. The web view maintains the aspect ratio of the captured content, but scales it to match the width you specify.

The default value of this property is `nil`, which returns an image whose size matches the original size of the captured rectangle.

## See Also

### Specifying the snapshot dimensions

var rect: CGRect

The portion of your web view to capture, specified as a rectangle in the view’s coordinate system.

