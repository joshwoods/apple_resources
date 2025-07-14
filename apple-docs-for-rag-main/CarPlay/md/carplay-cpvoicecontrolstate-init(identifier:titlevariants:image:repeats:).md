

- CarPlay
- CPVoiceControlState
-  init(identifier:titleVariants:image:repeats:) 

Initializer

# init(identifier:titleVariants:image:repeats:)

Creates a voice control state.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
init(
    identifier: String,
    titleVariants: [String]?,
    image: UIImage?,
    repeats: Bool
)
```

## Parameters 

`identifier`  

A string that your app uses to identify the state. You can activate the state by calling activateVoiceControlState(withIdentifier:), passing in the `identifier`.

`titleVariants`  

An array of title variants for the voice control state. When the system displays the title, it selects the title that best fits the available screen space, so arrange the titles from most to least preferred. Also, localize each title for display to the user, and be sure to include at least one title in the array.

`image`  

An image, no bigger than 150 pt x 150 pt, that the voice control template displays when it’s in this state. For an animated image, the system enforces a minimum cycle duration of 0.3 seconds, and a maximum cycle duration of 5 seconds.

`repeats`  

A Boolean value that indicates whether animation for `image` repeats indefinitely. Set to true to repeat the animation, or false to show the animation only once.

## Return Value

A newly initialized voice control state.

