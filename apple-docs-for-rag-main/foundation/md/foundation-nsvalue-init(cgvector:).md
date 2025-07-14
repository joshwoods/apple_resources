

- Foundation
- NSValue
-  init(CGVector:) 

Initializer

# init(CGVector:)

Creates a new value object containing the specified CoreGraphics vector structure.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(CGVector vector: CGVector)
```

``` source
init(cgVector vector: CGVector)
```

## Parameters 

`vector`  

The value for the new object.

## Return Value

A new value object that contains the vector information.

## See Also

### Related Documentation

struct CGVector

A structure that contains a two-dimensional vector.

### Working with CoreGraphics Geometry Values

init(CGPoint: CGPoint)

Creates a new value object containing the specified CoreGraphics point structure.

init(CGSize: CGSize)

Creates a new value object containing the specified CoreGraphics size structure.

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

