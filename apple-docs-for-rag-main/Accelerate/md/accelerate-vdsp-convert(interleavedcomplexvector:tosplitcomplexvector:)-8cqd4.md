

- Accelerate
- vDSP
-  convert(interleavedComplexVector:toSplitComplexVector:) 

Type Method

# convert(interleavedComplexVector:toSplitComplexVector:)

Converts the contents of an interleaved double-precision complex vector to a split complex vector.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static func convert(
    interleavedComplexVector: [DSPDoubleComplex],
    toSplitComplexVector splitComplexVector: inout DSPDoubleSplitComplex
)
```

## Parameters 

`interleavedComplexVector`  

The interleaved complex source vector.

`splitComplexVector`  

The split complex destination vector.

## See Also

### Converting interleaved-complex vectors to split-complex vectors

static func convert(interleavedComplexVector: [DSPComplex], toSplitComplexVector: inout DSPSplitComplex)

Converts the contents of an interleaved single-precision complex vector to a split complex vector.

