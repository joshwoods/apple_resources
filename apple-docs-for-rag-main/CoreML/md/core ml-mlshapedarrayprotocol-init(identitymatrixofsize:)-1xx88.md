

- Core ML
- MLShapedArrayProtocol
-  init(identityMatrixOfSize:) 

Initializer

# init(identityMatrixOfSize:)

Initialize as an identity matrix.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(identityMatrixOfSize size: Int)
```

Available when `Scalar` conforms to `BinaryFloatingPoint` and `Scalar.RawSignificand` conforms to `FixedWidthInteger`.

## Parameters 

`size`  

The size (order) of the matrix

## Discussion

The initializer creates a shaped array of shape size x size where the contents are zeros except array\[scalarAt: x, x\], which are ones.

