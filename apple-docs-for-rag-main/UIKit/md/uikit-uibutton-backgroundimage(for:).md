

- UIKit
- UIButton
-  backgroundImage(for:) 

Instance Method

# backgroundImage(for:)

Returns the background image used for a button state.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func backgroundImage(for state: UIControl.State) -> UIImage?
```

## Parameters 

`state`  

The state that uses the background image. Possible values are described in UIControl.State.

## Return Value

The background image used for the specified state.

## See Also

### Managing images and tint color

func image(for: UIControl.State) -> UIImage?

Returns the image used for a button state.

func setBackgroundImage(UIImage?, for: UIControl.State)

Sets the background image to use for the specified button state.

func setImage(UIImage?, for: UIControl.State)

Sets the image to use for the specified state.

func preferredSymbolConfigurationForImage(in: UIControl.State) -> UIImage.SymbolConfiguration?

Returns the preferred symbol configuration for a button state.

func setPreferredSymbolConfiguration(UIImage.SymbolConfiguration?, forImageIn: UIControl.State)

Sets the preferred symbol configuration for a button state.

var tintColor: UIColor!

The tint color to apply to the button title and image.

