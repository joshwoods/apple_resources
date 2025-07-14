

- Metal Performance Shaders
-  MPSNDArrayDescriptor 

Class

# MPSNDArrayDescriptor

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class MPSNDArrayDescriptor : NSObject
```

## Topics

### Initializers

init(dataType: MPSDataType, dimensionCount: Int, dimensionSizes: UnsafeMutablePointer&lt;Int>)

init(dataType: MPSDataType, shape: [NSNumber])

### Instance Properties

var dataType: MPSDataType

var numberOfDimensions: Int

var preferPackedRows: Bool

### Instance Methods

func dimensionOrder() -> vector_uchar16

func getShape() -> [NSNumber]

func length(ofDimension: Int) -> Int

func permute(withDimensionOrder: UnsafeMutablePointer&lt;Int>)

func reshape(withDimensionCount: Int, dimensionSizes: UnsafeMutablePointer&lt;Int>)

func reshape(withShape: [NSNumber])

func sliceDimension(Int, withSubrange: MPSDimensionSlice)

func sliceRange(forDimension: Int) -> MPSDimensionSlice

func transposeDimension(Int, withDimension: Int)

## Relationships

### Inherits From

- NSObject

