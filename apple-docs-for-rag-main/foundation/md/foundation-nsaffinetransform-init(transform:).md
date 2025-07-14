

- Foundation
- NSAffineTransform
-  init(transform:) 

Initializer

# init(transform:)

Initializes the receiver’s matrix using another transform object.

Mac Catalyst 13.0+macOS 10.0+

**macOS**

``` source
convenience init(transform: AffineTransform)
```

**Mac Catalyst**

``` source
convenience init(transform: NSAffineTransform)
```

## Parameters 

`transform`  

The transform object whose matrix values should be copied to this object.

## Return Value

A new transform object initialized with the matrix values of `aTransform`.

## See Also

### Creating an Affine Transform

init()

Initializes an affine transform matrix to the identity matrix.

