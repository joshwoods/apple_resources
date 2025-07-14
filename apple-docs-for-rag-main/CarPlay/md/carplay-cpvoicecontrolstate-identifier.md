

- CarPlay
- CPVoiceControlState
-  identifier 

Instance Property

# identifier

The string that your app uses to identify the voice control state.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
var identifier: String { get }
```

## Discussion

Use identifier when calling the activateVoiceControlState(withIdentifier:) method to activate the voice control state.

## See Also

### Getting State Information

var titleVariants: [String]?

The array of title variants for the voice control state.

var image: UIImage?

The image displayed while the voice control template is in this state.

var repeats: Bool

A Boolean value that indicates whether the display of an animated image repeats the animation sequence indefinitely.

