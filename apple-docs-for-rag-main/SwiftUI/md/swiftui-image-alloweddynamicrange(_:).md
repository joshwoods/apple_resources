

- SwiftUI
- Image
-  allowedDynamicRange(\_:) 

Instance Method

# allowedDynamicRange(\_:)

Returns a new image configured with the specified allowed dynamic range.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
func allowedDynamicRange(_ range: Image.DynamicRange?) -> Image
```

## Parameters 

`range`  

The requested dynamic range, or nil to restore the default allowed range.

## Return Value

A new image.

## Discussion

The following example enables HDR rendering for a specific image view, assuming that the image has an HDR (ITU-R 2100) color space and the output device supports it:

```
Image("hdr-asset").allowedDynamicRange(.high)
```

## See Also

### Specifying dynamic range

var allowedDynamicRange: Image.DynamicRange?

The allowed dynamic range for the view, or nil.

struct DynamicRange

