

- Core Graphics
-  CGPathElement 

Structure

# CGPathElement

A data structure that provides information about a path element.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct CGPathElement
```

## Topics

### Initializers

init(type: CGPathElementType, points: UnsafeMutablePointer&lt;CGPoint>)

### Instance Properties

var points: UnsafeMutablePointer&lt;CGPoint>

An array of one or more points that serve as arguments.

var type: CGPathElementType

An element type (or operation).

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Applying a Function to the Elements of a Path

func apply(info: UnsafeMutableRawPointer?, function: CGPathApplierFunction)

For each element in a graphics path, calls a custom applier function.

typealias CGPathApplierFunction

Defines a callback function that can view an element in a graphics path.

enum CGPathElementType

The type of element found in a path.

