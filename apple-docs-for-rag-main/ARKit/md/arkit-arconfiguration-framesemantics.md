

- ARKit
- ARConfiguration
-  frameSemantics 

Instance Property

# frameSemantics

The set of active semantics on the frame.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
var frameSemantics: ARConfiguration.FrameSemantics { get set }
```

## Discussion

You can choose whether ARKit reports information about a particular per-frame metric, or *semantic*. Before enabling a frame sementic, call supportsFrameSemantics(_:) to ensure device support.

### Enable 2D Body Detection

To get information about the 2D location of a person that ARKit recognizes in a frame, you enable the bodyDetection frame semantic.

```
if let config = mySession.configuration as? ARBodyTrackingConfiguration {
    config.frameSemantics.insert(.bodyDetection)
    // Run the configuration to effect a frame semantics change.
    mySession.run(config)
}

```

### Enable People Occlusion

People occlusion is a feature that enables people in the camera feed to cover your app’s virtual content.

To indicate that a person should overlap your app’s virtual content when the person is closer to the camera than the virtual content, add the personSegmentationWithDepth option to your configuration’s frame semantics.

```
if let config = mySession.configuration as? ARWorldTrackingConfiguration {
    config.frameSemantics.insert(.personSegmentationWithDepth)
    // Run the configuration to effect a frame semantics change.
    mySession.run(config)
}

```

To indicate that a person should overlap your app’s virtual content regardless of the person’s depth in the scene, use the personSegmentation frame semantic instead. This option is particularly appropriate for green-screen scenarios.

Standard renderers (ARView, and ARSCNView) implement people occlusion for you. See Occluding virtual content with people for a sample app that demonstrates people occlusion in RealityKit.

If you implement your own renderer, use segmentationBuffer and estimatedDepthData to implement people occlusion yourself. ARMatteGenerator helps you by providing masks. For a sample app that demonstrates matte generator and people occlusion, see Effecting People Occlusion in Custom Renderers.

If you enable Scene Reconstruction, ARKit adjusts the mesh according to any people ARKit may detect in the camera feed. ARKit removes any part of the scene mesh that overlaps with people, as defined by the with- or without-depth frame semantics. For more information about scene reconstruction, see Visualizing and interacting with a reconstructed scene.

## See Also

### Enabling frame features

struct FrameSemantics

Types of optional frame features you can enable in your app.

class func supportsFrameSemantics(ARConfiguration.FrameSemantics) -> Bool

Checks whether a particular feature is supported.

