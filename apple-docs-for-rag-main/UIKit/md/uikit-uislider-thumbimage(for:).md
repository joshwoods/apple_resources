

- UIKit
- UISlider
-  thumbImage(for:) 

Instance Method

# thumbImage(for:)

Returns the thumb image associated with the specified control state.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func thumbImage(for state: UIControl.State) -> UIImage?
```

## Parameters 

`state`  

The control state whose thumb image you want to use. Specify a single control state value for this parameter.

## Return Value

The thumb image associated with the specified state, or `nil` if an appropriate image could not be retrieved. This method might return `nil` if you specify multiple control states in the `state` parameter. For a description of track and thumb images, see Customize the slider’s appearance.

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

func setThumbImage(UIImage?, for: UIControl.State)

Assigns a thumb image to the specified control states.

