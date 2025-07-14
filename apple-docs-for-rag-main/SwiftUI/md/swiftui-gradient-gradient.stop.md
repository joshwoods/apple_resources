

- SwiftUI
- Gradient
-  Gradient.Stop 

Structure

# Gradient.Stop

One color stop in the gradient.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@frozen
struct Stop
```

## Topics

### Creating a gradient stop

init(color: Color, location: CGFloat)

Creates a color stop with a color and location.

### Configuring a gradient stop

var color: Color

The color for the stop.

var location: CGFloat

The parametric location of the stop.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Creating a gradient from stops

init(stops: [Gradient.Stop])

Creates a gradient from an array of color stops.

var stops: [Gradient.Stop]

The array of color stops.

