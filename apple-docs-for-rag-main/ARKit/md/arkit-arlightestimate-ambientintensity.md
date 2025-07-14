

- ARKit
- ARLightEstimate
-  ambientIntensity 

Instance Property

# ambientIntensity

The estimated intensity, in lumens, of ambient light throughout the scene.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
var ambientIntensity: CGFloat { get }
```

## Discussion

This value is based on the internal exposure compensation of the camera device, and scaled to be appropriate for use in rendering architectures that use realistic lighting metrics. A value of 1000 represents “neutral” lighting.

For example, you can pass this value directly to the intensity property of a SceneKit ambient light for lighting results that roughly match those of the real-world scene captured by the device camera. (However, passing this value to SceneKit is generally not necessary; the ARSCNView class automatically sets SceneKit lighting based on this value.)

## See Also

### Examining Light Parameters

var ambientColorTemperature: CGFloat

The estimated color temperature, in degrees Kelvin, of ambient light throughout the scene.

