

- Media Player
- MPVolumeView
-  volumeSliderRect(forBounds:) 

Instance Method

# volumeSliderRect(forBounds:)

Returns the drawing rectangle for the slider’s track.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func volumeSliderRect(forBounds bounds: CGRect) -> CGRect
```

## Parameters 

`bounds`  

The bounding rectangle of the receiver.

## Return Value

The computed drawing rectangle for the volume slider track. This rectangle corresponds to the entire length of the track between the minimum and maximum value images.

## Discussion

The system uses the rectangle to scale the track and thumb images during drawing.

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

func volumeThumbImage(for: UIControl.State) -> UIImage?

Returns the thumb image associated with the specified control state.

func volumeThumbRect(forBounds: CGRect, volumeSliderRect: CGRect, value: Float) -> CGRect

Returns the drawing rectangle for the volume slider’s thumb image.

