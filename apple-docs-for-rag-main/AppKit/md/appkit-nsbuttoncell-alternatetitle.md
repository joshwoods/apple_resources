

- AppKit
- NSButtonCell
-  alternateTitle 

Instance Property

# alternateTitle

The string displayed by the button when it’s in its alternate state.

macOS

``` source
@MainActor
var alternateTitle: String { get set }
```

## Discussion

The value of this property is the string that appears on the button when it’s in its alternate state, or the empty string if the button doesn’t display an alternate title. Note that some button types don’t display an alternate title. By default, a button’s alternate title is “Button.”

## See Also

### Related Documentation

var font: NSFont?

The font that the cell uses to display text.

func setButtonType(NSButton.ButtonType)

Sets how the button highlights while pressed and how it shows its state.

### Setting Titles

var attributedAlternateTitle: NSAttributedString

The title displayed by the button when it’s in its alternate state, as an attributed string.

var attributedTitle: NSAttributedString

The title displayed by the button when it’s in its normal state as an attributed string.

var title: String!

The title displayed on the button when it’s in its normal state.

