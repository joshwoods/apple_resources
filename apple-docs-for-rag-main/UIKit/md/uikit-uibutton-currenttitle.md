

- UIKit
- UIButton
-  currentTitle 

Instance Property

# currentTitle

The current title that is displayed on the button.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var currentTitle: String? { get }
```

## Discussion

The value for this property is set automatically whenever the button state changes. For states that do not have a custom title string associated with them, this method returns the title that is currently displayed, which is typically the one associated with the normal state. The value may be `nil`.

## See Also

### Related Documentation

var titleLabel: UILabel?

A view that displays the value of the `currentTitle` property for a button.

func setTitle(String?, for: UIControl.State)

Sets the title to use for the specified state.

### Getting the current state

var buttonType: UIButton.ButtonType

The button type.

var currentAttributedTitle: NSAttributedString?

The current styled title that is displayed on the button.

var currentTitleColor: UIColor

The color used to display the title.

var currentTitleShadowColor: UIColor?

The color of the title’s shadow.

var currentImage: UIImage?

The current image displayed on the button.

var currentBackgroundImage: UIImage?

The current background image displayed on the button.

var currentPreferredSymbolConfiguration: UIImage.SymbolConfiguration?

The current symbol size, style, and weight.

var imageView: UIImageView?

The button’s image view.

var subtitleLabel: UILabel?

The label that displays the text of the subtitle.

