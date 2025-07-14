

- Metal
- MTLRenderCommandEncoder
-  setStencilStoreAction(\_:) 

Instance Method

# setStencilStoreAction(\_:)

Configures the store action for the stencil attachment.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
func setStencilStoreAction(_ storeAction: MTLStoreAction)
```

**Required**

## Parameters 

`storeAction`  

A store action for the stencil attachment that can’t be MTLStoreAction.unknown.

## Discussion

This method changes the render command encoder’s store action for the stencil attachment. You can assign the default store action for the stencil attachment by configuring the storeAction property of its MTLRenderPassStencilAttachmentDescriptor (see MTLRenderPassDescriptor and its stencilAttachment property).

Important

You need to call this method before calling the encoder’s endEncoding() method, but only if the stencil attachment’s storeAction property is equal to MTLStoreAction.unknown.

## See Also

### Configuring the Actions for Attachments

func setColorStoreAction(MTLStoreAction, index: Int)

Configures the store action for a color attachment.

**Required**

func setColorStoreActionOptions(MTLStoreActionOptions, index: Int)

Configures the store action options for a color attachment.

**Required**

func setDepthStoreAction(MTLStoreAction)

Configures the store action for the depth attachment.

**Required**

func setDepthStoreActionOptions(MTLStoreActionOptions)

Configures the store action options for the depth attachment.

**Required**

func setStencilStoreActionOptions(MTLStoreActionOptions)

Configures the store action options for the stencil attachment.

**Required**

