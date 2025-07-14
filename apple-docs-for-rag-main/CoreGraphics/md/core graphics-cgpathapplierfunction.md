

- Core Graphics
-  CGPathApplierFunction 

Type Alias

# CGPathApplierFunction

Defines a callback function that can view an element in a graphics path.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias CGPathApplierFunction = (UnsafeMutableRawPointer?, UnsafePointer) -> Void
```

## Discussion

See also apply(info:function:).

## See Also

### Applying a Function to the Elements of a Path

func apply(info: UnsafeMutableRawPointer?, function: CGPathApplierFunction)

For each element in a graphics path, calls a custom applier function.

struct CGPathElement

A data structure that provides information about a path element.

enum CGPathElementType

The type of element found in a path.

