

- RealityKit
- PhotogrammetrySession
- PhotogrammetrySession.Configuration
-  sampleOrdering 

Instance Property

# sampleOrdering

The order of the image samples.

iOS 17.0+iPadOS 17.0+Mac Catalyst 15.0+macOS 12.0+

``` source
var sampleOrdering: PhotogrammetrySession.Configuration.SampleOrdering
```

## Discussion

By default, RealityKit assumes that image samples aren’t in any particular order. If you’re providing the images in order, with adjacent images next to each other, specifying PhotogrammetrySession.Configuration.SampleOrdering.sequential for this value may result in better performance.

This setting has no impact on the quality of the produced object.

## See Also

### Configuring sample ordering

enum SampleOrdering

The ordering of samples.

