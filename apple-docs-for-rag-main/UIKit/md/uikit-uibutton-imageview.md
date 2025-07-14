

- UIKit
- UIButton
-  imageView 

Instance Property

# imageView

The button’s image view.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var imageView: UIImageView? { get }
```

## Discussion

Although this property is read-only, its own properties are read/write. Use these properties to configure the appearance and behavior of the button’s view. For example:

```
UIButton *button                   = [UIButton buttonWithType: UIButtonTypeSystem];
button.imageView.exclusiveTouch    = YES;
```

The `imageView` property returns a value even if the button has not been displayed yet. The value of the property is `nil` for system buttons.

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

var subtitleLabel: UILabel?

The label that displays the text of the subtitle.

