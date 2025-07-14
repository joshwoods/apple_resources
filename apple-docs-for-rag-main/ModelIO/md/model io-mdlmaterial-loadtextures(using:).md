

- Model I/O
- MDLMaterial
-  loadTextures(using:) 

Instance Method

# loadTextures(using:)

Loads textures using resolver for string paths and NSURLs.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
func loadTextures(using resolver: any MDLAssetResolver)
```

## Parameters 

`resolver`  

If non-nil, the resolver converts stringValues or NSURLs to MDLTextureSampler values.

## Discussion

Iterates all material properties. If there are string values or NSURL values, and you can resolve the values as textures, then MDLTextureSampler values replaces the string and NSURL values.

## See Also

### Working with textures using resolvers

func resolveTextures(with: any MDLAssetResolver)

Resolves all texture string paths as NSURLs with resolver.

