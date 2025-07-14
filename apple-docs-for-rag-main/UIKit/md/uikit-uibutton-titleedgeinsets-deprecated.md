

- UIKit
- UIButton
-  titleEdgeInsets Deprecated

Instance Property

# titleEdgeInsets

The inset or outset margins for the rectangle around the button’s title text.

iOS 2.0–15.0DeprecatediPadOS 2.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedtvOS 2.0–15.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
var titleEdgeInsets: UIEdgeInsets { get set }
```

## Discussion

Use this property to resize and reposition the effective drawing rectangle for the button title. You can specify a different value for each of the four insets (top, left, bottom, right). A positive value shrinks, or insets, that edge—moving it closer to the center of the button. A negative value expands, or outsets, that edge. Use the init(top:left:bottom:right:) function to construct a value for this property. The default value is zero.

The insets you specify are applied to the title rectangle after that rectangle has been sized to fit the button’s text. Thus, positive inset values may actually clip the title text.

This property is used only for positioning the title during layout. The button does not use this property to determine intrinsicContentSize and sizeThatFits(_:).

## See Also

### Edge insets

var contentEdgeInsets: UIEdgeInsets

The inset or outset margins for the rectangle surrounding all of the button’s content.

Deprecated

var imageEdgeInsets: UIEdgeInsets

The inset or outset margins for the rectangle around the button’s image.

Deprecated

