

- Accelerate
- vDSP
-  convert(splitComplexVector:toInterleavedComplexVector:) 

Type Method

# convert(splitComplexVector:toInterleavedComplexVector:)

Converts the contents of a split double-precision complex vector to an interleaved vector.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static func convert(
    splitComplexVector: DSPDoubleSplitComplex,
    toInterleavedComplexVector interleavedComplexVector: inout [DSPDoubleComplex]
)
```

## Parameters 

`splitComplexVector`  

The split-complex source vector.

`interleavedComplexVector`  

The interleaved-complex destination vector.

## See Also

### Converting split-complex vectors to interleaved-complex vectors

static func convert(splitComplexVector: DSPSplitComplex, toInterleavedComplexVector: inout [DSPComplex])

Converts the contents of a split single-precision complex vector to an interleaved vector.

