

- Metal
- MTLTexture
-  makeSharedTextureHandle() 

Instance Method

# makeSharedTextureHandle()

Creates a new texture handle from a shareable texture.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.14+tvOS 13.0+visionOS 1.0+

``` source
func makeSharedTextureHandle() -> MTLSharedTextureHandle?
```

**Required**

## Discussion

If the texture is not shareable, this method returns `nil`.

