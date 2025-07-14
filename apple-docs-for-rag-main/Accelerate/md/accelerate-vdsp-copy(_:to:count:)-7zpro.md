

- Accelerate
- vDSP
-  copy(\_:to:count:) 

Type Method

# copy(\_:to:count:)

Copies a complex double-precision vector.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static func copy(
    _ source: DSPDoubleSplitComplex,
    to destination: inout DSPDoubleSplitComplex,
    count: Int
)
```

## Parameters 

`source`  

The source complex vector.

`destination`  

The destination complex vector.

`count`  

The number of complex elements in the source and destination vectors.

## Discussion

The following code copies the complex elements in the source to the destination:

```
    let realSrc = UnsafeMutableBufferPointer.allocate(capacity: 4)
    _ = realSrc.initialize(from: [0, 2, 4, 6])

    let imagSrc = UnsafeMutableBufferPointer.allocate(capacity: 4)
    _ = imagSrc.initialize(from: [1, 3, 5, 7])

    let source = DSPDoubleSplitComplex(realp: realSrc.baseAddress!,
                                       imagp: imagSrc.baseAddress!)

    let realDst = UnsafeMutableBufferPointer.allocate(capacity: 4)
    let imagDst = UnsafeMutableBufferPointer.allocate(capacity: 4)

    var destination = DSPDoubleSplitComplex(realp: realDst.baseAddress!,
                                            imagp: imagDst.baseAddress!)

    vDSP.copy(source, to: &destination, count: 4)

    print(Array(realDst)) // Prints "[0.0, 2.0, 4.0, 6.0]".
    print(Array(imagDst)) // Prints "[1.0, 3.0, 5.0, 7.0]".
```

## See Also

### Vector copying functions

static func copy(DSPSplitComplex, to: inout DSPSplitComplex, count: Int)

Copies a complex single-precision vector.

