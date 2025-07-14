

- PHASE
- PHASESpatialPipeline
-  init(flags:) 

Initializer

# init(flags:)

Creates a spatial pipeline with the specified flags.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
init?(flags: PHASESpatialPipeline.Flags)
```

## Parameters 

`flags`  

An array of sound-resonance effects to include in the spatial pipeline’s output. The framework adds an entry to the entries property for each element that the app includes in this collection.

## Discussion

This initializer returns `nil` for a `nil` `flags` argument.

## See Also

### Creating a Spatial Pipeline

struct Flags

Sound resonance options for a spatial pipeline.

