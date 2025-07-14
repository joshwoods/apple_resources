

- Metal
- MTLDepthStencilDescriptor
-  depthCompareFunction 

Instance Property

# depthCompareFunction

The comparison that is performed between a fragment’s depth value and the depth value in the attachment, which determines whether to discard the fragment.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
var depthCompareFunction: MTLCompareFunction { get set }
```

## Discussion

The default value is MTLCompareFunction.always, which indicates that the depth test always passes and the fragment remains a candidate to replace the data at the specified location. For more information on possible values, see MTLCompareFunction.

## See Also

### Related Documentation

Metal Shading Language Guide

Metal Programming Guide

### Specifying Depth Operations

var isDepthWriteEnabled: Bool

A Boolean value that indicates whether depth values can be written to the depth attachment.

