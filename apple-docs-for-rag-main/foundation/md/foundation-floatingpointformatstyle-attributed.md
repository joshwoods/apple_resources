

- Foundation
- FloatingPointFormatStyle
-  attributed 

Instance Property

# attributed

An attributed format style based on the floating-point format style.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var attributed: FloatingPointFormatStyle.Attributed { get }
```

## Discussion

Use this modifier to create a FloatingPointFormatStyle.Attributed instance, which formats values as AttributedString instances. These attributed strings contain attributes from the AttributeScopes.FoundationAttributes.NumberFormatAttributes attribute scope. Use these attributes to determine which runs of the attributed string represent different parts of the formatted value.

The following example finds runs of the attributed string that represent different parts of a formatted currency, and adds additional attributes like foregroundColor and inlinePresentationIntent.

```
func attributedPrice(price: Double) -> AttributedString {
    var attributedPrice = price.formatted(
        .currency(code: "USD")
        .attributed)

    for run in attributedPrice.runs {
        if run.attributes.numberSymbol == .currency ||
            run.attributes.numberSymbol == .decimalSeparator {
            attributedPrice[run.range].foregroundColor = .red
        }
        if run.attributes.numberPart == .integer ||
            run.attributes.numberPart == .fraction {
            attributedPrice[run.range].inlinePresentationIntent = [.stronglyEmphasized]
        }
    }
    return attributedPrice
}
```

User interface frameworks like SwiftUI can use these attributes when presenting the attributed string, as seen here:

## See Also

### Creating attributed strings

struct Attributed

A format style that converts integers into attributed strings.

