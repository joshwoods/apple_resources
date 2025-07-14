

- Foundation
- NSValue
-  init(CGSize:) 

Initializer

# init(CGSize:)

Creates a new value object containing the specified CoreGraphics size structure.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(CGSize size: CGSize)
```

``` source
init(cgSize size: CGSize)
```

## Parameters 

`size`  

The value for the new object.

## Return Value

A new value object that contains the size information.

## See Also

### Related Documentation

struct CGSize

A structure that contains width and height values.

### Working with CoreGraphics Geometry Values

init(CGPoint: CGPoint)

Creates a new value object containing the specified CoreGraphics point structure.

init(CGVector: CGVector)

Creates a new value object containing the specified CoreGraphics vector structure.

init(CGRect: CGRect)

Creates a new value object containing the specified CoreGraphics rectangle structure.

init(CGAffineTransform: CGAffineTransform)

Creates a new value object containing the specified CoreGraphics affine transform structure.

var cgPointValue: CGPoint

Returns the CoreGraphics point structure representation of the value.

var cgVectorValue: CGVector

Returns the CoreGraphics vector structure representation of the value.

var cgSizeValue: CGSize

Returns the CoreGraphics size structure representation of the value.

var cgRectValue: CGRect

Returns the CoreGraphics rectangle structure representation of the value.

var cgAffineTransformValue: CGAffineTransform

Returns the CoreGraphics affine transform representation of the value.

