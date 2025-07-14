

- SwiftUI
- Image
-  Image.DynamicRange 

Structure

# Image.DynamicRange

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
struct DynamicRange
```

## Topics

### Getting dynamic range values

static let standard: Image.DynamicRange

Restrict the image content dynamic range to the standard range.

static let high: Image.DynamicRange

Allow image content to use an unrestricted extended range.

static let constrainedHigh: Image.DynamicRange

Allow image content to use some extended range. This is appropriate for placing HDR content next to SDR content.

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### Specifying dynamic range

func allowedDynamicRange(Image.DynamicRange?) -> Image

Returns a new image configured with the specified allowed dynamic range.

var allowedDynamicRange: Image.DynamicRange?

The allowed dynamic range for the view, or nil.

