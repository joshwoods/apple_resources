

- RealityKit
- DirectionalLightComponent
- DirectionalLightComponent.Shadow
- DirectionalLightComponent.Shadow.ShadowProjectionType
-  DirectionalLightComponent.Shadow.ShadowProjectionType.automatic(maximumDistance:) 

Case

# DirectionalLightComponent.Shadow.ShadowProjectionType.automatic(maximumDistance:)

Shadow projection is automatically fit with the camera frustum, range is within maximumDistance from camera

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
case automatic(maximumDistance: Float = 5)
```

## See Also

### Shadow projection types

case fixed(zNear: Float, zFar: Float, orthographicScale: Float)

Shadow projection is manually set up with near plane, far plane, and orthographicScale for width and height

