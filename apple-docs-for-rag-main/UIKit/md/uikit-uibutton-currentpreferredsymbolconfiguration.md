

- UIKit
- UIButton
-  currentPreferredSymbolConfiguration 

Instance Property

# currentPreferredSymbolConfiguration

The current symbol size, style, and weight.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
var currentPreferredSymbolConfiguration: UIImage.SymbolConfiguration? { get }
```

## Discussion

This can be `nil` or `unspecifiedConfiguration`, which is essentially the same as `nil` but more explicit.

## See Also

### Getting the current state

var buttonType: UIButton.ButtonType

The button type.

var currentTitle: String?

The current title that is displayed on the button.

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

var imageView: UIImageView?

The button’s image view.

var subtitleLabel: UILabel?

The label that displays the text of the subtitle.

