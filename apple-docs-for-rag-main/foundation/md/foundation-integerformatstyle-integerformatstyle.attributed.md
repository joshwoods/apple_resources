

- Foundation
- IntegerFormatStyle
-  IntegerFormatStyle.Attributed 

Structure

# IntegerFormatStyle.Attributed

A format style that converts integers into attributed strings.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct Attributed
```

Available when `Value` conforms to `BinaryInteger`.

## Overview

Use the attributed modifier on an IntegerFormatStyle to create a format style of this type.

The attributed strings that this format style creates contain attributes from the AttributeScopes.FoundationAttributes.NumberFormatAttributes attribute scope. Use these attributes to determine which runs of the attributed string represent different parts of the formatted value.

The following example finds runs of the attributed string that represent different parts of a formatted currency, and adds additional attributes like foregroundColor and inlinePresentationIntent.

```
func attributedPrice(price: Decimal) -> AttributedString {
    var attributedPrice = price.formatted(
        .currency(code: "USD")
        .attributed)

    for run in attributedPrice.runs {
        if run.attributes.numberSymbol == .currency ||
            run.attributes.numberSymbol == .decimalSeparator  {
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

## Topics

### Formatting an integer

func format(Value) -> AttributedString

Formats an integer, using this style.

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- FormatStyle
- Hashable
- Sendable

## See Also

### Creating attributed strings

var attributed: IntegerFormatStyle&lt;Value>.Attributed

An attributed format style based on the integer format style.

