

- SwiftUI
- Text
- Text.Layout
-  Text.Layout.DrawingOptions 

Structure

# Text.Layout.DrawingOptions

Option flags used when drawing `Text.Layout` lines or runs into a graphics context.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@frozen
struct DrawingOptions
```

## Topics

### Type Properties

static var disablesSubpixelQuantization: Text.Layout.DrawingOptions

If set, subpixel quantization requested by the text engine is disabled. This can be useful for text that will be animated to prevent it jittering.

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

