

- UIKit
- UIButton
-  setBackgroundImage(\_:for:) 

Instance Method

# setBackgroundImage(\_:for:)

Sets the background image to use for the specified button state.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func setBackgroundImage(
    _ image: UIImage?,
    for state: UIControl.State
)
```

## Parameters 

`image`  

The background image to use for the specified state.

`state`  

The state that uses the specified image. The values are described in UIControl.State.

## Discussion

In general, if a property is not specified for a state, the default is to use the normal value. If the normal value is not set, then the property defaults to a system value. Therefore, at a minimum, you should set the value for the normal state.

## See Also

### Managing images and tint color

func backgroundImage(for: UIControl.State) -> UIImage?

Returns the background image used for a button state.

func image(for: UIControl.State) -> UIImage?

Returns the image used for a button state.

func setImage(UIImage?, for: UIControl.State)

Sets the image to use for the specified state.

func preferredSymbolConfigurationForImage(in: UIControl.State) -> UIImage.SymbolConfiguration?

Returns the preferred symbol configuration for a button state.

func setPreferredSymbolConfiguration(UIImage.SymbolConfiguration?, forImageIn: UIControl.State)

Sets the preferred symbol configuration for a button state.

var tintColor: UIColor!

The tint color to apply to the button title and image.

