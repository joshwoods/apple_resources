

- Metal
- MTLCounterSampleBufferError
- MTLCounterSampleBufferError.Code
-  MTLCounterSampleBufferError.Code.invalid 

Case

# MTLCounterSampleBufferError.Code.invalid

An error code that indicates when a counter-sample buffer descriptor has at least one invalid property.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
case invalid
```

## Discussion

This error applies to the MTLDevice protocol’s makeCounterSampleBuffer(descriptor:) method and its MTLCounterSampleBufferDescriptor parameter.

## See Also

### Error Codes

case outOfMemory

An error code that indicates the GPU device doesn’t have sufficient memory to create a counter sample buffer.

case `internal`

An error code that indicates the Metal framework has an internal problem.

case outOfMemory

An error code that indicates the GPU device doesn’t have sufficient memory to create a counter sample buffer.

case `internal`

An error code that indicates the Metal framework has an internal problem.

