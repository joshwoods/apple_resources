

- Foundation
- NSAffineTransform
-  transformStruct 

Instance Property

# transformStruct

The matrix coefficients stored as the transformation matrix.

Mac Catalyst 13.0+macOS 10.0+

``` source
var transformStruct: NSAffineTransformStruct { get set }
```

## Discussion

The matrix is of the form shown in Transform Mathematics, and the six-element structure defined by the NSAffineTransformStruct structure is of the form:

```
{m11, m12, m21, m22, tX, tY}
```

The NSAffineTransformStruct structure is an alternate representation of a transformation matrix that can be used to specify matrix values directly.

## See Also

### Related Documentation

convenience init(transform: NSAffineTransform)

Initializes the receiver’s matrix using another transform object.

### Accessing the Transformation Matrix

struct NSAffineTransformStruct

A structure that defines the three-by-three matrix that performs an affine transform between two coordinate systems.

