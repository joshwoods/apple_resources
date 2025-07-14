

- Metal
- MTLRenderPassDepthAttachmentDescriptor
-  depthResolveFilter 

Instance Property

# depthResolveFilter

The filter used for an MSAA depth resolve operation.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.14+tvOS 9.0+visionOS 1.0+

``` source
var depthResolveFilter: MTLMultisampleDepthResolveFilter { get set }
```

## Discussion

The default value is MTLMultisampleDepthResolveFilter.sample0.

