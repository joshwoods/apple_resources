

- UIKit
- UISlider
-  minimumValueImage 

Instance Property

# minimumValueImage

The image that represents the slider’s minimum value.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var minimumValueImage: UIImage? { get set }
```

## Discussion

The image you specify must fit within the bounding rectangle returned by the minimumValueImageRect(forBounds:) method. If it doesn’t, the slider scales the image to fit. In addition, the slider lengthens or shortens its track as needed to accommodate the image in its bounding rectangle.

Because *minimum* is a semantic concept, in a right-to-left user interface, the slider automatically flips the image placement, always placing it at the leading end of the slider’s track.

The default value of this property is `nil`.

Important

This property isn’t available when the user interface idiom is UIUserInterfaceIdiom.mac and behavioralStyle is UIBehavioralStyle.mac — setting it while in this state throws an exception.

## See Also

### Changing the slider’s appearance

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

func setThumbImage(UIImage?, for: UIControl.State)

Assigns a thumb image to the specified control states.

