

- Core Animation
- CAMetalDrawable
-  texture 

Instance Property

# texture

A Metal texture object that contains the drawable’s contents.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
var texture: any MTLTexture { get }
```

**Required**

## Discussion

Use this object to configure a MTLRenderPipelineColorAttachmentDescriptor object to render to the drawable object.

