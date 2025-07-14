

- ARKit
- ARWorldTrackingConfiguration
- ARWorldTrackingConfiguration.EnvironmentTexturing
-  ARWorldTrackingConfiguration.EnvironmentTexturing.automatic 

Case

# ARWorldTrackingConfiguration.EnvironmentTexturing.automatic

The framework automatically determines when and where to generate environment textures.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
case automatic
```

## Discussion

When you use this environmentTexturing option, ARKit automatically chooses positions in the scene to generate environment textures based on the camera imagery it has collected and the other anchors you’ve placed.

If you display AR content using ARSCNView, SceneKit automatically retrieves texture maps from probe anchors and uses them to light the scene. Otherwise, use a delegate method such as session(_:didUpdate:) to find out when the probe anchor’s texture has been updated and access the environmentTexture property.

