

- Metal
- MTLParallelRenderCommandEncoder
-  setStencilStoreAction(\_:) 

Instance Method

# setStencilStoreAction(\_:)

Specifies a known store action to replace the initial MTLStoreAction.unknown value specified for a given stencil attachment.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
func setStencilStoreAction(_ storeAction: MTLStoreAction)
```

**Required**

## Parameters 

`storeAction`  

The desired store action for the stencil attachment. This value must not be MTLStoreAction.unknown.

## Discussion

If the store action for the given stencil attachment was set to MTLStoreAction.unknown when the parallel render command encoder was created, you must call this method to specify another store action before you call the endEncoding() method.

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

func setStencilStoreActionOptions(MTLStoreActionOptions)

Specifies known store action options for a given stencil attachment.

**Required**

