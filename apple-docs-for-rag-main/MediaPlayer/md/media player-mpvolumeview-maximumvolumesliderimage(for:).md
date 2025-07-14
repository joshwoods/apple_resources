

- Media Player
- MPVolumeView
-  maximumVolumeSliderImage(for:) 

Instance Method

# maximumVolumeSliderImage(for:)

Returns the maximum volume image associated with the specified control state.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func maximumVolumeSliderImage(for state: UIControl.State) -> UIImage?
```

## Parameters 

`state`  

The control state whose maximum volume image you want. You should specify only one control state value for this parameter.

## Return Value

The maximum volume image associated with the specified state, or nil if an appropriate image could not be retrieved. This method might return nil if you specify multiple control states in the `state` parameter.

## Discussion

For a description of slider and thumb images, see Customizing the volume slider’s appearance.

## See Also

### Customizing the volume slider

func minimumVolumeSliderImage(for: UIControl.State) -> UIImage?

Returns the minimum volume image associated with the specified control state.

func setMaximumVolumeSliderImage(UIImage?, for: UIControl.State)

Assigns a maximum volume slider image to the specified control states.

func setMinimumVolumeSliderImage(UIImage?, for: UIControl.State)

Assigns a minimum volume slider image to the specified control states.

func setVolumeThumbImage(UIImage?, for: UIControl.State)

Assigns a thumb image to the specified control states.

func volumeSliderRect(forBounds: CGRect) -> CGRect

Returns the drawing rectangle for the slider’s track.

func volumeThumbImage(for: UIControl.State) -> UIImage?

Returns the thumb image associated with the specified control state.

func volumeThumbRect(forBounds: CGRect, volumeSliderRect: CGRect, value: Float) -> CGRect

Returns the drawing rectangle for the volume slider’s thumb image.

