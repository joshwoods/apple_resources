

- UIKit
- UIButton
-  subtitleLabel 

Instance Property

# subtitleLabel

The label that displays the text of the subtitle.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
@MainActor
var subtitleLabel: UILabel? { get }
```

## Discussion

If configuration is `nil`, this property is `nil`.

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

var currentPreferredSymbolConfiguration: UIImage.SymbolConfiguration?

The current symbol size, style, and weight.

var imageView: UIImageView?

The button’s image view.

