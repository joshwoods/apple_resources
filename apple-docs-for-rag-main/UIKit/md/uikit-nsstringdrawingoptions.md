

- UIKit
-  NSStringDrawingOptions 

Structure

# NSStringDrawingOptions

Constants that specify the rendering options for drawing a string.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct NSStringDrawingOptions
```

## Topics

### Constants

static var usesLineFragmentOrigin: NSStringDrawingOptions

Uses the line fragment origin instead of the baseline origin.

static var usesFontLeading: NSStringDrawingOptions

Uses the font leading for calculating line heights.

static var usesDeviceMetrics: NSStringDrawingOptions

Uses image glyph bounds instead of typographic bounds.

static var truncatesLastVisibleLine: NSStringDrawingOptions

Truncates and adds the ellipsis character to the last visible line if the text doesn’t fit into the specified bounds.

### Initializer

init(rawValue: Int)

Creates a structure that specifies the rendering options for drawing a string.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Strings

class NSStringDrawingContext

An object that manages metrics for drawing attributed strings.

enum UIBaselineAdjustment

Vertical adjustment options.

