

- Metal
- MTLRenderCommandEncoder
-  setDepthStoreAction(\_:) 

Instance Method

# setDepthStoreAction(\_:)

Configures the store action for the depth attachment.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
func setDepthStoreAction(_ storeAction: MTLStoreAction)
```

**Required**

## Parameters 

`storeAction`  

A store action for the depth attachment that can’t be MTLStoreAction.unknown.

## Discussion

This method changes the render command encoder’s store action for the depth attachment. You can assign the default store action for the depth attachment by configuring the storeAction property of its MTLRenderPassDepthAttachmentDescriptor (see MTLRenderPassDescriptor and its depthAttachment property).

Important

You need to call this method before calling the encoder’s endEncoding() method, but only if the depth attachment’s storeAction property is equal to MTLStoreAction.unknown.

## See Also

### Configuring the Actions for Attachments

func setColorStoreAction(MTLStoreAction, index: Int)

Configures the store action for a color attachment.

**Required**

func setColorStoreActionOptions(MTLStoreActionOptions, index: Int)

Configures the store action options for a color attachment.

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

