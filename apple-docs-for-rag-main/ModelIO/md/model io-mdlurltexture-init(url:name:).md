

- Model I/O
- MDLURLTexture
-  init(url:name:) 

Initializer

# init(url:name:)

Initializes a texture that loads its texel data from a file at the specified URL.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
init(
    url URL: URL,
    name: String?
)
```

## Parameters 

`URL`  

The URL from which to load texture data.

`name`  

The name property for the new texture object.

## Return Value

A new URL-backed texture.

## Discussion

This initializer does not load texel data from the URL; the MDLURLTexture class automatically loads data and caches it for reuse when you use one of the MDLTexture methods listed in Accessing Texture Data.

