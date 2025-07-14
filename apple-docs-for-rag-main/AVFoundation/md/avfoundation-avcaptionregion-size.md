

- AVFoundation
- AVCaptionRegion
-  size 

Instance Property

# size

The height and width of the region.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
var size: AVCaptionSize { get }
```

## Discussion

CEA608 closed captions limit the height property’s value to 1 cell, except when the value of its scroll property is AVCaptionRegion.Scroll.rollUp. In this case, the height property’s value must be 2, 3 or 4 cells.

Note

The caption size has an unspecified height and width when the region doesn’t have width or height information.

## See Also

### Accessing the Size

struct AVCaptionSize

A structure that defines the height and width of a caption.

