

- ScreenCaptureKit
- SCContentFilter
-  streamType Deprecated

Instance Property

# streamType

The type of the streaming content.

Mac Catalyst 17.0–17.2DeprecatedmacOS 14.0–14.2Deprecated

``` source
var streamType: SCStreamType { get }
```

Deprecated

Use style instead

## Discussion

Note

Use the style property instead, which provides additional information about the content.

## See Also

### Filter properties

var contentRect: CGRect

The size and location of the content to filter, in screen points.

var pointPixelScale: Float

The scaling factor used to translate screen points into pixels.

enum SCStreamType

The display type of the presented stream.

Deprecated

var style: SCShareableContentStyle

The display style of the sharable content.

