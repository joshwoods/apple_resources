

- Media Player
- MPVolumeView
-  volumeThumbRect(forBounds:volumeSliderRect:value:) 

Instance Method

# volumeThumbRect(forBounds:volumeSliderRect:value:)

Returns the drawing rectangle for the volume slider’s thumb image.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func volumeThumbRect(
    forBounds bounds: CGRect,
    volumeSliderRect rect: CGRect,
    value: Float
) -> CGRect
```

## Parameters 

`bounds`  

The bounding rectangle of the thumb image.

`rect`  

The drawing rectangle for the receiver’s track, as returned by the volumeSliderRect(forBounds:) method.

`value`  

The current value of the volume slider.

## Return Value

The computed drawing rectangle for the thumb image.

## Discussion

The rectangle you return should reflect the size of your thumb image and its current position on the slider’s track.

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

func volumeThumbImage(for: UIControl.State) -> UIImage?

Returns the thumb image associated with the specified control state.

