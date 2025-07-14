

- AVFoundation
- AVCaptionRegion
-  origin 

Instance Property

# origin

The region’s top-left position.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
var origin: AVCaptionPoint { get }
```

## Discussion

The caption’s origin may not provide undefined x and y values, which indicates the region doesn’t have positioning information for that dimension.

## See Also

### Accessing the Location

struct AVCaptionPoint

A structure that defines the origin point for a caption.

