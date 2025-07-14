

- UIKit
- UIButton
-  titleLabel 

Instance Property

# titleLabel

A view that displays the value of the `currentTitle` property for a button.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var titleLabel: UILabel? { get }
```

## Discussion

Although this property is read-only, its own properties are read/write. Use these properties primarily to configure the text of the button. For example:

```
UIButton *button                  = [UIButton buttonWithType: UIButtonTypeSystem];
button.titleLabel.font            = [UIFont systemFontOfSize: 12];
button.titleLabel.lineBreakMode   = NSLineBreakByTruncatingTail;
```

Do not use the label object to set the text color or the shadow color. Instead, use the setTitleColor(_:for:) and setTitleShadowColor(_:for:) methods of this class to make those changes. To set the actual text of the label, use setTitle(_:for:) (`button.titleLabel.text` does not let you set the text).

The `titleLabel` property returns a value even if the button has not been displayed yet. The value of the property is `nil` for system buttons.

## See Also

### Related Documentation

var currentTitle: String?

The current title that is displayed on the button.

### Managing the title

func title(for: UIControl.State) -> String?

Returns the title associated with the specified state.

func setTitle(String?, for: UIControl.State)

Sets the title to use for the specified state.

func attributedTitle(for: UIControl.State) -> NSAttributedString?

Returns the styled title associated with the specified state.

func setAttributedTitle(NSAttributedString?, for: UIControl.State)

Sets the styled title to use for the specified state.

func titleColor(for: UIControl.State) -> UIColor?

Returns the title color used for a state.

func setTitleColor(UIColor?, for: UIControl.State)

Sets the color of the title to use for the specified state.

func titleShadowColor(for: UIControl.State) -> UIColor?

Returns the shadow color of the title used for a state.

func setTitleShadowColor(UIColor?, for: UIControl.State)

Sets the color of the title shadow to use for the specified state.

