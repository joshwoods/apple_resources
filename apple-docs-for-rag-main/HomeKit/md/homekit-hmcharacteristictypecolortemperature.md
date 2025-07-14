

- HomeKit
-  HMCharacteristicTypeColorTemperature 

Global Variable

# HMCharacteristicTypeColorTemperature

The color temperature of a light.

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
let HMCharacteristicTypeColorTemperature: String
```

## Discussion

The corresponding value is an integer representing the color temperature in micro-reciprocal degrees (mired), which is 1,000,000 divided by the color temperature in kelvins. For example, to emulate a traditional tungsten light with a color temperature of 3200 K, use a mired value of about 312.

## See Also

### Light

let HMCharacteristicTypeCurrentLightLevel: String

The current light level.

let HMCharacteristicTypeHue: String

The hue of the color used by a light.

let HMCharacteristicTypeBrightness: String

The brightness of a light.

let HMCharacteristicTypeSaturation: String

The saturation of the color used by a light.

