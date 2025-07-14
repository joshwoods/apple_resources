

- Swift Charts
- AxisTick
-  AxisTick.Length 

Structure

# AxisTick.Length

Describes the length of a tick.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct Length
```

## Topics

### Type Properties

static var automatic: AxisTick.Length

Automatically determines the tick length.

static var label: AxisTick.Length

Describes a tick that extends to its associated label.

static var longestLabel: AxisTick.Length

Describes a tick that extends to the longest label on the axis.

### Type Methods

static func label(extendPastBy: CGFloat) -> AxisTick.Length

Describes a tick that extends to its associated label, with the given additional length.

static func longestLabel(extendPastBy: CGFloat) -> AxisTick.Length

Describes a tick that extends to the longest label on the axis, with the given additional length.

## Relationships

### Conforms To

- CustomStringConvertible

