

- UIKit
- UISlider
-  trackRect(forBounds:) 

Instance Method

# trackRect(forBounds:)

Returns the drawing rectangle for the slider’s track.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func trackRect(forBounds bounds: CGRect) -> CGRect
```

## Parameters 

`bounds`  

The bounding rectangle of the slider.

## Return Value

The computed drawing rectangle for the track. This rectangle corresponds to the entire length of the track between the minimum and maximum value images.

## Discussion

You do not call this method directly. Instead, you override it when you want to customize the track rectangle, returning a different rectangle. The returned rectangle is used to scale the track and thumb images during drawing.

## See Also

### Overrides for subclasses

func maximumValueImageRect(forBounds: CGRect) -> CGRect

Returns the drawing rectangle for the maximum value image.

func minimumValueImageRect(forBounds: CGRect) -> CGRect

Returns the drawing rectangle for the minimum value image.

func thumbRect(forBounds: CGRect, trackRect: CGRect, value: Float) -> CGRect

Returns the drawing rectangle for the slider’s thumb image.

