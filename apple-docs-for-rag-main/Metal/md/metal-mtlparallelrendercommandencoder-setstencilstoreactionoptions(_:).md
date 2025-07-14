

- Metal
- MTLParallelRenderCommandEncoder
-  setStencilStoreActionOptions(\_:) 

Instance Method

# setStencilStoreActionOptions(\_:)

Specifies known store action options for a given stencil attachment.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
func setStencilStoreActionOptions(_ storeActionOptions: MTLStoreActionOptions)
```

**Required**

## Parameters 

`storeActionOptions`  

The additional store action options for the stencil attachment.

## See Also

### Setting Render Pass State

func setColorStoreAction(MTLStoreAction, index: Int)

Specifies a known store action to replace the initial MTLStoreAction.unknown value specified for a given color attachment.

**Required**

func setColorStoreActionOptions(MTLStoreActionOptions, index: Int)

Specifies known store action options for a given color attachment.

**Required**

func setDepthStoreAction(MTLStoreAction)

Specifies a known store action to replace the initial MTLStoreAction.unknown value specified for a given depth attachment.

**Required**

func setDepthStoreActionOptions(MTLStoreActionOptions)

Specifies known store action options for a given depth attachment.

**Required**

func setStencilStoreAction(MTLStoreAction)

Specifies a known store action to replace the initial MTLStoreAction.unknown value specified for a given stencil attachment.

**Required**

