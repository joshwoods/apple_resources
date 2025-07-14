

- UIKit
- UISlider
-  thumbRect(forBounds:trackRect:value:) 

Instance Method

# thumbRect(forBounds:trackRect:value:)

Returns the drawing rectangle for the slider’s thumb image.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func thumbRect(
    forBounds bounds: CGRect,
    trackRect rect: CGRect,
    value: Float
) -> CGRect
```

## Parameters 

`bounds`  

The bounding rectangle of the slider.

`rect`  

The drawing rectangle for the slider’s track, as returned by the trackRect(forBounds:) method.

`value`  

The current value of the slider.

## Return Value

The computed drawing rectangle for the thumb image.

## Discussion

You do not call this method directly. Instead, you override it when you want to customize the thumb image’s drawing rectangle, returning a different rectangle. The rectangle you return must reflect the size of your thumb image and its current position on the slider’s track.

## See Also

### Overrides for subclasses

func maximumValueImageRect(forBounds: CGRect) -> CGRect

Returns the drawing rectangle for the maximum value image.

func minimumValueImageRect(forBounds: CGRect) -> CGRect

Returns the drawing rectangle for the minimum value image.

func trackRect(forBounds: CGRect) -> CGRect

Returns the drawing rectangle for the slider’s track.

