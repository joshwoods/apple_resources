

- UIKit
- UIButton
-  currentAttributedTitle 

Instance Property

# currentAttributedTitle

The current styled title that is displayed on the button.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var currentAttributedTitle: NSAttributedString? { get }
```

## Discussion

The value for this property reflects the title associated with the control’s current state. For states that do not have a custom title string associated with them, this method returns the attributed title that is currently displayed, which is typically the one associated with the normal state.

## See Also

### Getting the current state

var buttonType: UIButton.ButtonType

The button type.

var currentTitle: String?

The current title that is displayed on the button.

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

