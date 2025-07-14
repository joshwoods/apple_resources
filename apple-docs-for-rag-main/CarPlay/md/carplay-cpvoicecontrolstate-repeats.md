

- CarPlay
- CPVoiceControlState
-  repeats 

Instance Property

# repeats

A Boolean value that indicates whether the display of an animated image repeats the animation sequence indefinitely.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
var repeats: Bool { get }
```

## Discussion

The animation repeats when this property is true; otherwise, animation occurs only once.

## See Also

### Getting State Information

var identifier: String

The string that your app uses to identify the voice control state.

var titleVariants: [String]?

The array of title variants for the voice control state.

var image: UIImage?

The image displayed while the voice control template is in this state.

