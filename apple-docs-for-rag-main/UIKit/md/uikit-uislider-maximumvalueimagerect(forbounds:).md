

- UIKit
- UISlider
-  maximumValueImageRect(forBounds:) 

Instance Method

# maximumValueImageRect(forBounds:)

Returns the drawing rectangle for the maximum value image.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func maximumValueImageRect(forBounds bounds: CGRect) -> CGRect
```

## Parameters 

`bounds`  

The bounding rectangle of the slider.

## Return Value

The computed drawing rectangle for the image.

## Discussion

You do not call this method directly. Instead, you override it when you want to customize the rectangle in which the maximum value image is drawn, returning a different rectangle. If you make x-axis adjustments, be sure to take into account the automatic flipping of maximumValueImage in a right-to-left user interface; the maximum image is always shown at the trailing end of the slider’s track. See the Internationalization and Localization Guide for further information about supporting right-to-left languages.

## See Also

### Overrides for subclasses

func minimumValueImageRect(forBounds: CGRect) -> CGRect

Returns the drawing rectangle for the minimum value image.

func trackRect(forBounds: CGRect) -> CGRect

Returns the drawing rectangle for the slider’s track.

func thumbRect(forBounds: CGRect, trackRect: CGRect, value: Float) -> CGRect

Returns the drawing rectangle for the slider’s thumb image.

