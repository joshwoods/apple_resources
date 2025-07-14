

- AVFoundation
- AVCaptionRegion
-  AVCaptionRegion.Scroll 

Enumeration

# AVCaptionRegion.Scroll

Constants that indicate the scrolling effects the system applies to a region.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
enum Scroll
```

## Topics

### Scroll Values

case none

A type that indicates no scrolling.

case rollUp

A type that indicates a roll-up scroll effect.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Accessing the Scroll Mode

var scroll: AVCaptionRegion.Scroll

The scroll mode of the region.

