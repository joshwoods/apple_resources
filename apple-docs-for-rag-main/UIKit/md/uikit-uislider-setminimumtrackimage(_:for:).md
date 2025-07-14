

- UIKit
- UISlider
-  setMinimumTrackImage(\_:for:) 

Instance Method

# setMinimumTrackImage(\_:for:)

Assigns a minimum track image to the specified control states.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func setMinimumTrackImage(
    _ image: UIImage?,
    for state: UIControl.State
)
```

## Parameters 

`image`  

The minimum track image to associate with the specified states.

`state`  

The control state with which to associate the image.

## Discussion

Because the movement of the slider’s thumb changes the width of the area occupied by the minimum track image, the image width changes accordingly. To accommodate this requirement, specify track images as stretchable images that can grow or shrink to fill the available space. For information about how to create stretchable images, see UIImage.

When you specify a custom minimum track image, the slider ignores the custom minimum track tint color, if any.

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

func setThumbImage(UIImage?, for: UIControl.State)

Assigns a thumb image to the specified control states.

