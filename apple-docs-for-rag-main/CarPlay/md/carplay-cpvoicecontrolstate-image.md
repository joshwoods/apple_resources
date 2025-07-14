

- CarPlay
- CPVoiceControlState
-  image 

Instance Property

# image

The image displayed while the voice control template is in this state.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
var image: UIImage? { get }
```

## Discussion

For the animated images, the system enforces a minimum cycle duration of 0.3 seconds, and a maximum cycle duration of 5 seconds.

## See Also

### Getting State Information

var identifier: String

The string that your app uses to identify the voice control state.

var titleVariants: [String]?

The array of title variants for the voice control state.

var repeats: Bool

A Boolean value that indicates whether the display of an animated image repeats the animation sequence indefinitely.

