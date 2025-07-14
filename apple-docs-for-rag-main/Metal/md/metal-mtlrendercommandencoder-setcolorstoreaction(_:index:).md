

- Metal
- MTLRenderCommandEncoder
-  setColorStoreAction(\_:index:) 

Instance Method

# setColorStoreAction(\_:index:)

Configures the store action for a color attachment.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
func setColorStoreAction(
    _ storeAction: MTLStoreAction,
    index colorAttachmentIndex: Int
)
```

**Required**

## Parameters 

`storeAction`  

A store action for the color attachment that can’t be MTLStoreAction.unknown.

`colorAttachmentIndex`  

The index of a color attachment.

## Discussion

This method changes the render command encoder’s store action for a color attachment. You can assign the default store action for a color attachment by configuring the storeAction property of its MTLRenderPassColorAttachmentDescriptor (see MTLRenderPassDescriptor and its colorAttachments property).

Important

You need to call this method before calling the encoder’s endEncoding() method, but only for color attachments with a storeAction property equal to MTLStoreAction.unknown.

## See Also

### Configuring the Actions for Attachments

func setColorStoreActionOptions(MTLStoreActionOptions, index: Int)

Configures the store action options for a color attachment.

**Required**

func setDepthStoreAction(MTLStoreAction)

Configures the store action for the depth attachment.

**Required**

func setDepthStoreActionOptions(MTLStoreActionOptions)

Configures the store action options for the depth attachment.

**Required**

func setStencilStoreAction(MTLStoreAction)

Configures the store action for the stencil attachment.

**Required**

func setStencilStoreActionOptions(MTLStoreActionOptions)

Configures the store action options for the stencil attachment.

**Required**

