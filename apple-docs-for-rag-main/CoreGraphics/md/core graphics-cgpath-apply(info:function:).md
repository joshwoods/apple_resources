

- Core Graphics
- CGPath
-  apply(info:function:) 

Instance Method

# apply(info:function:)

For each element in a graphics path, calls a custom applier function.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func apply(
    info: UnsafeMutableRawPointer?,
    function: CGPathApplierFunction
)
```

## Parameters 

`info`  

A pointer to the user data that Core Graphics will pass to the function being applied, or `NULL`.

`function`  

A pointer to the function to apply. See CGPathApplierFunction for more information.

## Discussion

For each element in the specified path, Core Graphics calls the applier function, which can examine (but not modify) the element.

## See Also

### Applying a Function to the Elements of a Path

typealias CGPathApplierFunction

Defines a callback function that can view an element in a graphics path.

struct CGPathElement

A data structure that provides information about a path element.

enum CGPathElementType

The type of element found in a path.

