

- UIKit
- UISlider
-  currentMaximumTrackImage 

Instance Property

# currentMaximumTrackImage

Contains the maximum track image currently being used to render the slider.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var currentMaximumTrackImage: UIImage? { get }
```

## Discussion

Sliders can have different track images for different control states. The active control state determines which maximum track image is stored in this property. To get the maximum track image for a different control state, use the maximumTrackImage(for:) method.

If no custom track images have been set using the setMaximumTrackImage(_:for:) method, this property contains the value `nil`. In that situation, the slider uses the default maximum track image for drawing.

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

