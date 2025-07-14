

- UIKit
- UISlider
-  maximumTrackTintColor 

Instance Property

# maximumTrackTintColor

The color used to tint the default maximum track images.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var maximumTrackTintColor: UIColor? { get set }
```

## Discussion

Setting this property resets the maximum track images back to the slider’s default images; any custom images are released by the slider. Setting this property to `nil` resets the tint color to the default and removes any custom maximum track images.

Important

This property isn’t available when the user interface idiom is UIUserInterfaceIdiom.mac and behavioralStyle is UIBehavioralStyle.mac — setting it while in this state throws an exception.

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

