

- Metal
- MTLRenderCommandEncoder
-  setStencilStoreActionOptions(\_:) 

Instance Method

# setStencilStoreActionOptions(\_:)

Configures the store action options for the stencil attachment.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
func setStencilStoreActionOptions(_ storeActionOptions: MTLStoreActionOptions)
```

**Required**

## Parameters 

`storeActionOptions`  

Additional options for the store action of the stencil attachment.

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

func setStencilStoreAction(MTLStoreAction)

Configures the store action for the stencil attachment.

**Required**

