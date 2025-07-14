

- Metal
- MTLCounterSampleBufferError
-  invalid 

Type Property

# invalid

An error code that indicates the descriptor for creating a counter sample buffer descriptor has an invalid property.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
static var invalid: MTLCounterSampleBufferError.Code { get }
```

## Discussion

This error applies to the MTLDevice protocol’s makeCounterSampleBuffer(descriptor:) method and its MTLCounterSampleBufferDescriptor parameter.

## See Also

### Error Code Values

static var outOfMemory: MTLCounterSampleBufferError.Code

An error code that indicates the GPU device doesn’t have sufficient memory to create a counter sample buffer.

static var `internal`: MTLCounterSampleBufferError.Code

An error code that indicates the Metal framework has an internal problem.

enum Code

The underlying error code type that indicates why a GPU driver can’t create a counter sample buffer.

