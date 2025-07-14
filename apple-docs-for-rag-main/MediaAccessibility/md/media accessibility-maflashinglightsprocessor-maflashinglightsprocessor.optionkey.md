

- Media Accessibility
- MAFlashingLightsProcessor
-  MAFlashingLightsProcessor.OptionKey 

Structure

# MAFlashingLightsProcessor.OptionKey

Options for the flashing lights processor.

iOS 17.0+iPadOS 17.0+Mac Catalyst 13.0+macOS 10.9+tvOS 17.0+visionOS 1.0+

``` source
struct OptionKey
```

## Topics

### Creating an options structure

init(String)

Creates an options structure.

init(rawValue: String)

Creates an options structure with the specified raw value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Processing video content

func processSurface(IOSurfaceRef, outSurface: inout IOSurfaceRef, timestamp: CFAbsoluteTime, options: [MAFlashingLightsProcessor.OptionKey : Any]?) -> MAFlashingLightsProcessor.Result

Processes a surface by analyzing pixels for sequences of flashing lights and mitigates them by dimming the content.

struct Result

An object that reports the result of the flashing lights processor.

