

- Metal
- MTLComputeCommandEncoder
-  setTextures(\_:range:) 

Instance Method

# setTextures(\_:range:)

Binds multiple textures to the texture argument table, allowing compute functions to access their data on the GPU.

iOS 8.0+iPadOS 8.0+Mac CatalystmacOS 10.11+tvOS 8.0+visionOS

``` source
func setTextures(
    _ textures: [(any MTLTexture)?],
    range: Range
)
```

## Parameters 

`textures`  

A list of MTLTexture instances to bind to the texture argument table.

`range`  

The texture table indices to bind each of the `textures` to, in the order they appear.

## Discussion

Important

This method requires that the number of instances in `textures` be the same as the length of `range`.

## See Also

### Encoding Textures

func setTexture((any MTLTexture)?, index: Int)

Binds a texture to the texture argument table, allowing compute kernels to access its data on the GPU.

**Required**

