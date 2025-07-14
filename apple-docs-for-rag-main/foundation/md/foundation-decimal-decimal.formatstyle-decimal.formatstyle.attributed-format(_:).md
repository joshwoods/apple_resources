

- Foundation
- Decimal
- Decimal.FormatStyle
- Decimal.FormatStyle.Attributed
-  format(\_:) 

Instance Method

# format(\_:)

Formats a decimal value, using this style.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func format(_ value: Decimal) -> AttributedString
```

## Parameters 

`value`  

The decimal value to format.

## Return Value

An attributed string representation of `value`, formatted according to the style’s configuration. The returned string contains attributes from the AttributeScopes.FoundationAttributes.NumberFormatAttributes attribute scope to indicate runs formatted by this format style.

