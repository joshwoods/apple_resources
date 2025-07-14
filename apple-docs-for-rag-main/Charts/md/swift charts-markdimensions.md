

- Swift Charts
-  MarkDimensions 

Structure

# MarkDimensions

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct MarkDimensions
```

## Topics

### Initializers

init(floatLiteral: Double)

Creates a constant width or height from a floating point value.

init(integerLiteral: Int)

Creates a constant width or height from an integer.

### Type Properties

static var automatic: MarkDimensions&lt;DataElement>

A dimension that determines its value automatically.

### Type Methods

static func fixed(CGFloat) -> MarkDimensions&lt;DataElement>

A constant dimension.

static func fixed(KeyPath&lt;DataElement, CGFloat>) -> MarkDimensions&lt;DataElement>

A constant dimension.

static func inset(KeyPath&lt;DataElement, CGFloat>) -> MarkDimensions&lt;DataElement>

A dimension that’s the step size minus the specified inset value on each side.

static func inset(CGFloat) -> MarkDimensions&lt;DataElement>

A dimension that’s the step size minus the specified inset value on each side.

static func ratio(CGFloat) -> MarkDimensions&lt;DataElement>

A dimension that’s proportional to the scale step size, using the specified ratio.

static func ratio(KeyPath&lt;DataElement, CGFloat>) -> MarkDimensions&lt;DataElement>

A dimension that’s proportional to the scale step size, using the specified ratio.

## Relationships

### Conforms To

- ExpressibleByFloatLiteral
- ExpressibleByIntegerLiteral

