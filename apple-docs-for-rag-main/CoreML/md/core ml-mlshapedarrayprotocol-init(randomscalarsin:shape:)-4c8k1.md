

- Core ML
- MLShapedArrayProtocol
-  init(randomScalarsIn:shape:) 

Initializer

# init(randomScalarsIn:shape:)

Initialize the shaped array with random scalar values.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(
    randomScalarsIn range: Range,
    shape: [Int]
)
```

Available when `Scalar` conforms to `BinaryFloatingPoint` and `Scalar.RawSignificand` conforms to `FixedWidthInteger`.

## Parameters 

`range`  

The value range of each scalar

`shape`  

The shape of the shaped array

