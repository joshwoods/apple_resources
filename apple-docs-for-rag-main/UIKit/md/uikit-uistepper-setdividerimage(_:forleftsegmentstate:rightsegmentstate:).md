

- UIKit
- UIStepper
-  setDividerImage(\_:forLeftSegmentState:rightSegmentState:) 

Instance Method

# setDividerImage(\_:forLeftSegmentState:rightSegmentState:)

Sets the image to use for the given combination of left and right states.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func setDividerImage(
    _ image: UIImage?,
    forLeftSegmentState leftState: UIControl.State,
    rightSegmentState rightState: UIControl.State
)
```

## Parameters 

`image`  

The divider image to use.

`leftState`  

The state of the left side of the control.

`rightState`  

The state of the right side of the control.

## See Also

### Customizing appearance

func backgroundImage(for: UIControl.State) -> UIImage?

Returns the background image associated with the specified control state.

func setBackgroundImage(UIImage?, for: UIControl.State)

Sets the background image for the control when it’s in the specified state.

func decrementImage(for: UIControl.State) -> UIImage?

Returns the image used for the decrement glyph of the control.

func setDecrementImage(UIImage?, for: UIControl.State)

Sets the image to use for the decrement glyph of the control.

func dividerImage(forLeftSegmentState: UIControl.State, rightSegmentState: UIControl.State) -> UIImage?

Returns the divider image for the given combination of left and right states.

func incrementImage(for: UIControl.State) -> UIImage?

Returns the image used for the increment glyph of the control.

func setIncrementImage(UIImage?, for: UIControl.State)

Sets the image to use for the increment glyph of the control.

