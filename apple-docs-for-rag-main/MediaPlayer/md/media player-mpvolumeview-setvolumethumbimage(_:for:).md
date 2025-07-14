

- Media Player
- MPVolumeView
-  setVolumeThumbImage(\_:for:) 

Instance Method

# setVolumeThumbImage(\_:for:)

Assigns a thumb image to the specified control states.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func setVolumeThumbImage(
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

For a description of slider and thumb images, see Customizing the volume slider’s appearance.

## See Also

### Customizing the volume slider

func maximumVolumeSliderImage(for: UIControl.State) -> UIImage?

Returns the maximum volume image associated with the specified control state.

func minimumVolumeSliderImage(for: UIControl.State) -> UIImage?

Returns the minimum volume image associated with the specified control state.

func setMaximumVolumeSliderImage(UIImage?, for: UIControl.State)

Assigns a maximum volume slider image to the specified control states.

func setMinimumVolumeSliderImage(UIImage?, for: UIControl.State)

Assigns a minimum volume slider image to the specified control states.

func volumeSliderRect(forBounds: CGRect) -> CGRect

Returns the drawing rectangle for the slider’s track.

func volumeThumbImage(for: UIControl.State) -> UIImage?

Returns the thumb image associated with the specified control state.

func volumeThumbRect(forBounds: CGRect, volumeSliderRect: CGRect, value: Float) -> CGRect

Returns the drawing rectangle for the volume slider’s thumb image.

