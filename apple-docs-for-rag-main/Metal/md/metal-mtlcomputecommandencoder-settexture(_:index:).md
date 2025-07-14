

- Metal
- MTLComputeCommandEncoder
-  setTexture(\_:index:) 

Instance Method

# setTexture(\_:index:)

Binds a texture to the texture argument table, allowing compute kernels to access its data on the GPU.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
func setTexture(
    _ texture: (any MTLTexture)?,
    index: Int
)
```

**Required**

## Parameters 

`texture`  

An MTLTexture instance to bind to the texture argument table.

`index`  

The index the texture binds to in the texture argument table.

## See Also

### Encoding Textures

func setTextures([(any MTLTexture)?], range: Range&lt;Int>)

Binds multiple textures to the texture argument table, allowing compute functions to access their data on the GPU.

