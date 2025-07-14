

- Core Animation
-  CAScrollLayer 

Class

# CAScrollLayer

A layer that displays scrollable content larger than its own bounds.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
class CAScrollLayer
```

## Overview

The CAScrollLayer class is a subclass of CALayer that simplifies displaying a portion of a layer. The extent of the scrollable area of the CAScrollLayer is defined by the layout of its sublayers. The visible portion of the layer content is set by specifying the origin as a point or a rectangular area of the contents to be displayed. CAScrollLayer does not provide keyboard or mouse event-handling, nor does it provide visible scrollers.

## Topics

### Scrolling constraints

var scrollMode: CAScrollLayerScrollMode

Defines the axes in which the layer may be scrolled.

### Scrolling the layer

func scroll(to: CGPoint)

Changes the origin of the receiver to the specified point.

func scroll(to: CGRect)

Scroll the contents of the receiver to ensure that the rectangle is visible.

### Constants

Scroll Modes

These constants describe the supported scroll modes used by the scrollMode property.

## Relationships

### Inherits From

- CALayer

### Conforms To

- CAMediaTiming
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Advanced Layer Options

class CATiledLayer

A layer that provides a way to asynchronously provide tiles of the layer’s content, potentially cached at multiple levels of detail.

class CATransformLayer

Objects used to create true 3D layer hierarchies, rather than the flattened hierarchy rendering model used by other layer types.

class CAReplicatorLayer

A layer that creates a specified number of sublayer copies with varying geometric, temporal, and color transformations.

