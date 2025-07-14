

- SwiftUI
-  LegibilityWeight 

Enumeration

# LegibilityWeight

The Accessibility Bold Text user setting options.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
enum LegibilityWeight
```

## Overview

The app can’t override the user’s choice before iOS 16, tvOS 16 or watchOS 9.0.

## Topics

### Getting weights

case regular

Use regular font weight (no Accessibility Bold).

case bold

Use heavier font weight (force Accessibility Bold).

### Creating a weight

init?(UILegibilityWeight)

Creates a legibility weight from its UILegibilityWeight equivalent.

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### Improving legibility

var accessibilityShowButtonShapes: Bool

Whether the system preference for Show Button Shapes is enabled.

var accessibilityReduceTransparency: Bool

Whether the system preference for Reduce Transparency is enabled.

var legibilityWeight: LegibilityWeight?

The font weight to apply to text.

