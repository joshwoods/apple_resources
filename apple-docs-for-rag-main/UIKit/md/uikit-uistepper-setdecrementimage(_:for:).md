

- UIKit
- UIStepper
-  setDecrementImage(\_:for:) 

Instance Method

# setDecrementImage(\_:for:)

Sets the image to use for the decrement glyph of the control.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func setDecrementImage(
    _ image: UIImage?,
    for state: UIControl.State
)
```

## Parameters 

`image`  

The image to use for the decrement glyph.

`state`  

The control state in which you want to display the image.

## Discussion

The image you specify is used as a template image to create the final control. If you don’t specify a custom image, a minus (`-`) glyph is used.

## See Also

### Customizing appearance

func backgroundImage(for: UIControl.State) -> UIImage?

Returns the background image associated with the specified control state.

func setBackgroundImage(UIImage?, for: UIControl.State)

Sets the background image for the control when it’s in the specified state.

func decrementImage(for: UIControl.State) -> UIImage?

Returns the image used for the decrement glyph of the control.

func dividerImage(forLeftSegmentState: UIControl.State, rightSegmentState: UIControl.State) -> UIImage?

Returns the divider image for the given combination of left and right states.

func setDividerImage(UIImage?, forLeftSegmentState: UIControl.State, rightSegmentState: UIControl.State)

Sets the image to use for the given combination of left and right states.

func incrementImage(for: UIControl.State) -> UIImage?

Returns the image used for the increment glyph of the control.

func setIncrementImage(UIImage?, for: UIControl.State)

Sets the image to use for the increment glyph of the control.

