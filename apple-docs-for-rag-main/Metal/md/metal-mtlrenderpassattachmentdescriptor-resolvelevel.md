

- Metal
- MTLRenderPassAttachmentDescriptor
-  resolveLevel 

Instance Property

# resolveLevel

The mipmap level of the texture used for the multisample resolve action.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
var resolveLevel: Int { get set }
```

## Discussion

If the value of storeAction is set to MTLStoreAction.multisampleResolve or MTLStoreAction.storeAndMultisampleResolve, set this property to point to a mipmap in the resolve texture.

The default value is `0`.

## See Also

### Specifying the Texture to Resolve Multisample Data

var resolveTexture: (any MTLTexture)?

The destination texture used when resolving multisampled texture data into single sample values.

var resolveSlice: Int

The slice of the texture used for the multisample resolve action.

var resolveDepthPlane: Int

The depth plane of the texture used for the multisample resolve action.

