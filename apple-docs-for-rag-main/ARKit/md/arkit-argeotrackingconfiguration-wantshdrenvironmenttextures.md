

- ARKit
- ARGeoTrackingConfiguration
-  wantsHDREnvironmentTextures 

Instance Property

# wantsHDREnvironmentTextures

A flag that instructs the framework to create environment textures in HDR format.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
var wantsHDREnvironmentTextures: Bool { get set }
```

## Discussion

If you set environmentTexturing to `.automatic` in iOS 12 or later, ARKit gives you environment textures you cast on your app’s virtual content to create realistic reflections. By default, the framework sets wantsHDREnvironmentTextures to true. When your renderer supports HDR environment textures in iOS 13, it enables your lighting engine to output more colors, with a more realistic result.

Both ARView and ARSCNView support HDR environment textures. For more information, see Adding realistic reflections to an AR experience.

For a Metal app that doesn’t yet support HDR environment textures, you can use the following code to receive LDR environment textures until you’re ready to update your renderer for HDR.

```
if #available(iOS 13, *) { 
    configuration.wantsHDREnvironmentTextures = false
}
```

## See Also

### Creating Realistic Reflections

var environmentTexturing: ARWorldTrackingConfiguration.EnvironmentTexturing

An option that determines how the framework generates environment textures.

enum EnvironmentTexturing

The available environment texturing options for world tracking.

class AREnvironmentProbeAnchor

An object that provides environmental lighting information for a specific area of space in a world-tracking AR session.

