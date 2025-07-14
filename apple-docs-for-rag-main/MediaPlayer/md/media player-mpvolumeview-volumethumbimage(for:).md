

- Media Player
- MPVolumeView
-  volumeThumbImage(for:) 

Instance Method

# volumeThumbImage(for:)

Returns the thumb image associated with the specified control state.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func volumeThumbImage(for state: UIControl.State) -> UIImage?
```

## Parameters 

`state`  

The control state whose thumb image you want. You should specify only one control state value for this parameter.

## Return Value

The thumb image associated with the specified state, or nil if an appropriate image could not be retrieved. This method might return nil if you specify multiple control states in the state parameter.

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

func setVolumeThumbImage(UIImage?, for: UIControl.State)

Assigns a thumb image to the specified control states.

func volumeSliderRect(forBounds: CGRect) -> CGRect

Returns the drawing rectangle for the slider’s track.

func volumeThumbRect(forBounds: CGRect, volumeSliderRect: CGRect, value: Float) -> CGRect

Returns the drawing rectangle for the volume slider’s thumb image.

