

- Metal Performance Shaders
-  MPSNDArray 

Class

# MPSNDArray

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class MPSNDArray : NSObject
```

## Topics

### Initializers

init(buffer: any MTLBuffer, offset: Int, descriptor: MPSNDArrayDescriptor)

init(device: any MTLDevice, descriptor: MPSNDArrayDescriptor)

init(device: any MTLDevice, scalar: Double)

### Instance Properties

var dataType: MPSDataType

var dataTypeSize: Int

var device: any MTLDevice

var label: String?

var numberOfDimensions: Int

var parent: MPSNDArray?

### Instance Methods

func arrayView(with: MPSNDArrayDescriptor) -> MPSNDArray?

func arrayView(with: any MTLCommandBuffer, descriptor: MPSNDArrayDescriptor, aliasing: MPSAliasingStrategy) -> MPSNDArray?

func arrayView(withDimensionCount: Int, dimensionSizes: UnsafePointer&lt;Int>, strides: UnsafePointer&lt;Int>) -> MPSNDArray?

func arrayView(withShape: [NSNumber]?, strides: [NSNumber]) -> MPSNDArray?

func descriptor() -> MPSNDArrayDescriptor

func exportData(with: any MTLCommandBuffer, to: any MTLBuffer, destinationDataType: MPSDataType, offset: Int, rowStrides: UnsafeMutablePointer&lt;Int>?)

func exportData(with: any MTLCommandBuffer, to: [MPSImage], offset: MPSImageCoordinate)

func importData(with: any MTLCommandBuffer, from: [MPSImage], offset: MPSImageCoordinate)

func importData(with: any MTLCommandBuffer, from: any MTLBuffer, sourceDataType: MPSDataType, offset: Int, rowStrides: UnsafeMutablePointer&lt;Int>?)

func length(ofDimension: Int) -> Int

func readBytes(UnsafeMutableRawPointer, strideBytes: UnsafeMutablePointer&lt;Int>?)

func resourceSize() -> Int

func synchronize(on: any MTLCommandBuffer)

func userBuffer() -> (any MTLBuffer)?

func writeBytes(UnsafeMutableRawPointer, strideBytes: UnsafeMutablePointer&lt;Int>?)

### Type Methods

class func defaultAllocator() -> any MPSNDArrayAllocator

## Relationships

### Inherits From

- NSObject

