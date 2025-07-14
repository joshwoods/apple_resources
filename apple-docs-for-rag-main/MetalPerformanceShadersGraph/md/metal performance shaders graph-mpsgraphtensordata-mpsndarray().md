

- Metal Performance Shaders Graph
- MPSGraphTensorData
-  mpsndarray() 

Instance Method

# mpsndarray()

Return an mpsndarray object will copy contents if the contents are not stored in an MPS ndarray.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func mpsndarray() -> MPSNDArray
```

## Return Value

A valid MPSNDArray, or nil if allocation fails.

