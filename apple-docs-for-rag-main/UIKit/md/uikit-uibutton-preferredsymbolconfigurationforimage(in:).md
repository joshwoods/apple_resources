

- UIKit
- UIButton
-  preferredSymbolConfigurationForImage(in:) 

Instance Method

# preferredSymbolConfigurationForImage(in:)

Returns the preferred symbol configuration for a button state.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
func preferredSymbolConfigurationForImage(in state: UIControl.State) -> UIImage.SymbolConfiguration?
```

## Parameters 

`state`  

The state that uses the symbol configuration. Possible values are described in UIControl.State.

## See Also

### Managing images and tint color

func backgroundImage(for: UIControl.State) -> UIImage?

Returns the background image used for a button state.

func image(for: UIControl.State) -> UIImage?

Returns the image used for a button state.

func setBackgroundImage(UIImage?, for: UIControl.State)

Sets the background image to use for the specified button state.

func setImage(UIImage?, for: UIControl.State)

Sets the image to use for the specified state.

func setPreferredSymbolConfiguration(UIImage.SymbolConfiguration?, forImageIn: UIControl.State)

Sets the preferred symbol configuration for a button state.

var tintColor: UIColor!

The tint color to apply to the button title and image.

