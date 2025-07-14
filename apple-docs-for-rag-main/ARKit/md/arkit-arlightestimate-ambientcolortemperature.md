

- ARKit
- ARLightEstimate
-  ambientColorTemperature 

Instance Property

# ambientColorTemperature

The estimated color temperature, in degrees Kelvin, of ambient light throughout the scene.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
var ambientColorTemperature: CGFloat { get }
```

## Discussion

This value is based on the internal white balance compensation of the camera device, and scaled to be appropriate for use in rendering architectures that use realistic lighting metrics. A value of 6500 represents neutral (pure white) lighting; lower values indicate a “warmer” yellow or orange tint, and higher values indicate a “cooler” blue tint.

For example, you can pass this value directly to the temperature property of a SceneKit ambient light for lighting results that roughly match those of the real-world scene captured by the device camera. (However, passing this value to SceneKit is generally not necessary; the ARSCNView class automatically sets SceneKit lighting based on this value.)

## See Also

### Examining Light Parameters

var ambientIntensity: CGFloat

The estimated intensity, in lumens, of ambient light throughout the scene.

