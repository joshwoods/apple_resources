

- Model I/O
- MDLMaterial
-  resolveTextures(with:) 

Instance Method

# resolveTextures(with:)

Resolves all texture string paths as NSURLs with resolver.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
func resolveTextures(with resolver: any MDLAssetResolver)
```

## Parameters 

`resolver`  

If non-nil, the resolver converts stringValues or NSURLs to MDLTextureSampler values.

## Discussion

Iterates all material properties. If there are string values, they’re resolved into valid paths as NSURL values by the resolver.

## See Also

### Working with textures using resolvers

func loadTextures(using: any MDLAssetResolver)

Loads textures using resolver for string paths and NSURLs.

