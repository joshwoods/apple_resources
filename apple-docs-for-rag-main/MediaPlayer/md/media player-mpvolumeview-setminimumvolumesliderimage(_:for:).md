

- Media Player
- MPVolumeView
-  setMinimumVolumeSliderImage(\_:for:) 

Instance Method

# setMinimumVolumeSliderImage(\_:for:)

Assigns a minimum volume slider image to the specified control states.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func setMinimumVolumeSliderImage(
    _ image: UIImage?,
    for state: UIControl.State
)
```

## Parameters 

`image`  

The minimum volume slider image to associate with the specified states.

`state`  

The control state with which to associate the image.

## Discussion

The orientation of the track image must match the orientation of the slider control. To facilitate the stretching of the image to fill the space between the thumb and end point, track images are usually defined in three regions. A stretchable region sits between two end cap regions. The end caps define the portions of the image that remain as is and aren’t stretched. The stretchable region is a 1-point wide area between the end caps that the system can replicate to make the image appear longer.

To define the end cap sizes for a slider, assign an appropriate value to the image’s capInsets property. For more information about how this value defines the regions of the slider, see the UIImage.

For a description of slider and thumb images, see Customizing the volume slider’s appearance.

## See Also

### Customizing the volume slider

func maximumVolumeSliderImage(for: UIControl.State) -> UIImage?

Returns the maximum volume image associated with the specified control state.

func minimumVolumeSliderImage(for: UIControl.State) -> UIImage?

Returns the minimum volume image associated with the specified control state.

func setMaximumVolumeSliderImage(UIImage?, for: UIControl.State)

Assigns a maximum volume slider image to the specified control states.

func setVolumeThumbImage(UIImage?, for: UIControl.State)

Assigns a thumb image to the specified control states.

func volumeSliderRect(forBounds: CGRect) -> CGRect

Returns the drawing rectangle for the slider’s track.

func volumeThumbImage(for: UIControl.State) -> UIImage?

Returns the thumb image associated with the specified control state.

func volumeThumbRect(forBounds: CGRect, volumeSliderRect: CGRect, value: Float) -> CGRect

Returns the drawing rectangle for the volume slider’s thumb image.

