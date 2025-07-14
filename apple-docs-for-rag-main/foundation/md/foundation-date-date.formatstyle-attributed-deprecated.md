

- Foundation
- Date
- Date.FormatStyle
-  attributed Deprecated

Instance Property

# attributed

An attributed format style created from the date format style.

iOS 15.0–18.0DeprecatediPadOS 15.0–18.0DeprecatedMac Catalyst 15.0–18.0DeprecatedmacOS 12.0–15.0DeprecatedtvOS 15.0–18.0DeprecatedvisionOS 1.0+watchOS 8.0–11.0Deprecated

``` source
var attributed: Date.AttributedStyle { get }
```

Deprecated

Use attributedStyle instead

## Discussion

Use a Date.FormatStyle instance to customize the lexical representation of a date as a string. Use the format style’s attributed property to customize the visual representation of the date as a string. Attributed strings can represent the subcomponent characters, words, and phrases of a string with a custom combination of font size, weight, and color.

For example, the function below uses a date format style to create a custom lexical representation of a date, then retrieves an attributed string representation of the same date and applies a visual emphasis to the year component of the date.

```
// Applies visual emphasis to the year component of a formatted attributed date string.
private func makeAttributedString() -> AttributedString {
    let date = Date()
    let formatStyle = Date.FormatStyle(date: .abbreviated, time: .standard)
    var attributedString = formatStyle.attributed.format(date)
    for run in attributedString.runs {
        if let dateFieldAttribute = run.attributes.foundation.dateField,
           dateFieldAttribute == .year {
            // When you find a year, change its attributes.
            attributedString[run.range].inlinePresentationIntent = [.emphasized, .stronglyEmphasized]
        }
    }
    return attributedString
}
```

The expression `formatStyle.attributed.format(date)` above creates an attributed string representation of the date. This assigns instances of the AttributeScopes.FoundationAttributes.DateFieldAttribute to indicate ranges of the string that represent different date fields. The example then loops over the `AttributedString/runs` of the attributed string to find any run with the AttributeScopes.FoundationAttributes.DateFieldAttribute.Field.year attribute. When it finds one, it adds the inlinePresentationIntent attributes emphasized and stronglyEmphasized.

The runs of the resulting attributed string have the following attributes:

| Run Text | Attributes |
|----|----|
| Mar | AttributeScopes.FoundationAttributes.DateFieldAttribute.Field.month |
| 15 | AttributeScopes.FoundationAttributes.DateFieldAttribute.Field.day |
| 2022 | AttributeScopes.FoundationAttributes.DateFieldAttribute.Field.year  emphasized  stronglyEmphasized |
| 10 | AttributeScopes.FoundationAttributes.DateFieldAttribute.Field.hour |
| 06 | AttributeScopes.FoundationAttributes.DateFieldAttribute.Field.minute |
| 46 | AttributeScopes.FoundationAttributes.DateFieldAttribute.Field.second |
| AM | AttributeScopes.FoundationAttributes.DateFieldAttribute.Field.amPM |

If you create a SwiftUI Text view with this attributed string, SwiftUI renders the combination of emphasized and stronglyEmphasized attributes as bold, italicized text, as seen in the following screenshot.

## See Also

### Applying Visual Attributes to Dates

struct AttributedStyle

A structure that creates a locale-appropriate attributed string representation of a date instance.

Deprecated

