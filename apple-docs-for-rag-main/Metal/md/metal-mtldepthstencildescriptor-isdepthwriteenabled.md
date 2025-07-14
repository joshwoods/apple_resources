

- Metal
- MTLDepthStencilDescriptor
-  isDepthWriteEnabled 

Instance Property

# isDepthWriteEnabled

A Boolean value that indicates whether depth values can be written to the depth attachment.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
var isDepthWriteEnabled: Bool { get set }
```

## Discussion

The default value is false, which indicates the depth attachment is read-only.

## See Also

### Specifying Depth Operations

var depthCompareFunction: MTLCompareFunction

The comparison that is performed between a fragment’s depth value and the depth value in the attachment, which determines whether to discard the fragment.

