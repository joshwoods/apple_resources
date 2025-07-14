

- AppKit
- NSButtonCell
-  attributedAlternateTitle 

Instance Property

# attributedAlternateTitle

The title displayed by the button when it’s in its alternate state, as an attributed string.

macOS

``` source
@NSCopying @MainActor
var attributedAlternateTitle: NSAttributedString { get set }
```

## Discussion

The value of this property is the attributed string that appears on the button when it’s in its alternate state, or the empty string if the button doesn’t display an alternate title. Note that some button types don’t display an alternate title. By default, a button’s alternate title is “Button.”

Graphics attributes that are set on the cell (such as `backgroundColor`, `alignment`, `font`, and so on) are overridden when corresponding properties are set for the attributed string.

## See Also

### Related Documentation

var font: NSFont?

The font that the cell uses to display text.

func setButtonType(NSButton.ButtonType)

Sets how the button highlights while pressed and how it shows its state.

### Setting Titles

var alternateTitle: String

The string displayed by the button when it’s in its alternate state.

var attributedTitle: NSAttributedString

The title displayed by the button when it’s in its normal state as an attributed string.

var title: String!

The title displayed on the button when it’s in its normal state.

