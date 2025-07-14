

- UIKit
- UIButton
-  setPreferredSymbolConfiguration(\_:forImageIn:) 

Instance Method

# setPreferredSymbolConfiguration(\_:forImageIn:)

Sets the preferred symbol configuration for a button state.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
func setPreferredSymbolConfiguration(
    _ configuration: UIImage.SymbolConfiguration?,
    forImageIn state: UIControl.State
)
```

## Parameters 

`configuration`  

The image symbol configuration for the specified state.

`state`  

The state that uses the specified image symbol configuration. Possible values are described in UIControl.State.

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

func preferredSymbolConfigurationForImage(in: UIControl.State) -> UIImage.SymbolConfiguration?

Returns the preferred symbol configuration for a button state.

var tintColor: UIColor!

The tint color to apply to the button title and image.

