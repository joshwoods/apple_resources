

- RealityKit
- DirectionalLightComponent
- DirectionalLightComponent.Shadow
- DirectionalLightComponent.Shadow.ShadowProjectionType
-  DirectionalLightComponent.Shadow.ShadowProjectionType.fixed(zNear:zFar:orthographicScale:) 

Case

# DirectionalLightComponent.Shadow.ShadowProjectionType.fixed(zNear:zFar:orthographicScale:)

Shadow projection is manually set up with near plane, far plane, and orthographicScale for width and height

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
case fixed(
    zNear: Float = 0.01,
    zFar: Float = 10,
    orthographicScale: Float = 1
)
```

## See Also

### Shadow projection types

case automatic(maximumDistance: Float)

Shadow projection is automatically fit with the camera frustum, range is within maximumDistance from camera

