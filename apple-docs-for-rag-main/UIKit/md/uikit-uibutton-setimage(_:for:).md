

- UIKit
- UIButton
-  setImage(\_:for:) 

Instance Method

# setImage(\_:for:)

Sets the image to use for the specified state.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func setImage(
    _ image: UIImage?,
    for state: UIControl.State
)
```

## Parameters 

`image`  

The image to use for the specified state.

`state`  

The state that uses the specified image. The values are described in UIControl.State.

## Discussion

At a minimum, always set an image for the normal state when associating images to a button. If you don’t specify an image for the other states, the button uses the image associated with normal. If you don’t specify an image for the normal state, the button uses a system value.

Important

When the user interface idiom is UIUserInterfaceIdiom.mac and behavioralStyle is UIBehavioralStyle.mac, your app throws an exception if you use this method to set the image for any state other than normal.

## See Also

### Managing images and tint color

func backgroundImage(for: UIControl.State) -> UIImage?

Returns the background image used for a button state.

func image(for: UIControl.State) -> UIImage?

Returns the image used for a button state.

func setBackgroundImage(UIImage?, for: UIControl.State)

Sets the background image to use for the specified button state.

func preferredSymbolConfigurationForImage(in: UIControl.State) -> UIImage.SymbolConfiguration?

Returns the preferred symbol configuration for a button state.

func setPreferredSymbolConfiguration(UIImage.SymbolConfiguration?, forImageIn: UIControl.State)

Sets the preferred symbol configuration for a button state.

var tintColor: UIColor!

The tint color to apply to the button title and image.

