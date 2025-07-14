

- RealityKit
- ImageBasedLightComponent
-  ImageBasedLightComponent.Source 

Enumeration

# ImageBasedLightComponent.Source

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
enum Source
```

## Topics

### Enumeration Cases

case blend(EnvironmentResource, EnvironmentResource, Float)

Blending between 2 IBLs. The Float is in \[0; 1\]: 0 will use the first IBL and 1 will use the second.

case none

case single(EnvironmentResource)

## See Also

### Image-based lights

struct ImageBasedLightComponent

struct ImageBasedLightReceiverComponent

