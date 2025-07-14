

- Core Video
-  kCVReturnRetry 

Global Variable

# kCVReturnRetry

A scan hasn’t completely traversed the `CVBufferPool` due to a concurrent operation.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 4.0+

``` source
var kCVReturnRetry: CVReturn { get }
```

## Discussion

A result of `kCVReturnRetry` indicates that a client can retry the scan.

## See Also

### Buffer Pool

var kCVReturnInvalidPoolAttributes: CVReturn

A buffer pool cannot be created with the specified attributes.

var kCVReturnPoolAllocationFailed: CVReturn

Allocation for a buffer pool failed, most likely due to a lack of resources. Check to make sure your parameters are in range.

var kCVReturnWouldExceedAllocationThreshold: CVReturn

Allocation for a pixel buffer failed because the threshold value set for the kCVPixelBufferPoolAllocationThresholdKey key in the CVPixelBufferPoolCreatePixelBufferWithAuxAttributes(_:_:_:_:) function would be surpassed.

