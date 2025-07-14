

- Metal
- MTLParallelRenderCommandEncoder
-  makeRenderCommandEncoder() 

Instance Method

# makeRenderCommandEncoder()

Create an object that encodes commands that perform graphics rendering operations and may be assigned to a different thread.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
func makeRenderCommandEncoder() -> (any MTLRenderCommandEncoder)?
```

**Required**

## Return Value

A graphics rendering command encoder object

## Discussion

The rendering commands encoded by MTLRenderCommandEncoder objects are executed in the order in which the MTLRenderCommandEncoder objects are created, not in the order they are ended.

## See Also

### Related Documentation

Metal Shading Language Guide

Metal Programming Guide

