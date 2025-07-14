

- UIKit
- UISlider
-  setThumbImage(\_:for:) 

Instance Method

# setThumbImage(\_:for:)

Assigns a thumb image to the specified control states.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func setThumbImage(
    _ image: UIImage?,
    for state: UIControl.State
)
```

## Parameters 

`image`  

The thumb image to associate with the specified states.

`state`  

The control state with which to associate the image.

## Discussion

When you specify a custom thumb image, the slider ignores the custom thumb tint color, if any.

Important

This method isn’t available when the user interface idiom is UIUserInterfaceIdiom.mac and behavioralStyle is UIBehavioralStyle.mac — calling it while in this state throws an exception.

## See Also

### Changing the slider’s appearance

var minimumValueImage: UIImage?

The image that represents the slider’s minimum value.

var maximumValueImage: UIImage?

The image representing the slider’s maximum value.

var minimumTrackTintColor: UIColor?

The color used to tint the default minimum track images.

var currentMinimumTrackImage: UIImage?

The minimum track image currently being used to render the slider.

func minimumTrackImage(for: UIControl.State) -> UIImage?

Returns the minimum track image associated with the specified control state.

func setMinimumTrackImage(UIImage?, for: UIControl.State)

Assigns a minimum track image to the specified control states.

var maximumTrackTintColor: UIColor?

The color used to tint the default maximum track images.

var currentMaximumTrackImage: UIImage?

Contains the maximum track image currently being used to render the slider.

func maximumTrackImage(for: UIControl.State) -> UIImage?

Returns the maximum track image associated with the specified control state.

func setMaximumTrackImage(UIImage?, for: UIControl.State)

Assigns a maximum track image to the specified control states.

var thumbTintColor: UIColor?

The color used to tint the default thumb images.

var currentThumbImage: UIImage?

The thumb image currently being used to render the slider.

func thumbImage(for: UIControl.State) -> UIImage?

Returns the thumb image associated with the specified control state.

