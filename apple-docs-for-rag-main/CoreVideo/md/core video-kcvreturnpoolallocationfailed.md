

- Core Video
-  kCVReturnPoolAllocationFailed 

Global Variable

# kCVReturnPoolAllocationFailed

Allocation for a buffer pool failed, most likely due to a lack of resources. Check to make sure your parameters are in range.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 4.0+

``` source
var kCVReturnPoolAllocationFailed: CVReturn { get }
```

## See Also

### Buffer Pool

var kCVReturnRetry: CVReturn

A scan hasn’t completely traversed the `CVBufferPool` due to a concurrent operation.

var kCVReturnInvalidPoolAttributes: CVReturn

A buffer pool cannot be created with the specified attributes.

var kCVReturnWouldExceedAllocationThreshold: CVReturn

Allocation for a pixel buffer failed because the threshold value set for the kCVPixelBufferPoolAllocationThresholdKey key in the CVPixelBufferPoolCreatePixelBufferWithAuxAttributes(_:_:_:_:) function would be surpassed.

