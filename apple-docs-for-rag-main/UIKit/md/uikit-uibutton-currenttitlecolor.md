

- UIKit
- UIButton
-  currentTitleColor 

Instance Property

# currentTitleColor

The color used to display the title.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var currentTitleColor: UIColor { get }
```

## Discussion

This value is guaranteed not to be `nil`. The default value is `white`.

## See Also

### Getting the current state

var buttonType: UIButton.ButtonType

The button type.

var currentTitle: String?

The current title that is displayed on the button.

var currentAttributedTitle: NSAttributedString?

The current styled title that is displayed on the button.

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

