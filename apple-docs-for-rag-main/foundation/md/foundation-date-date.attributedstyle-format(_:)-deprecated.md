

- Foundation
- Date
- Date.AttributedStyle
-  format(\_:) Deprecated

Instance Method

# format(\_:)

Creates a locale-aware attributed string representation from a date value.

iOS 15.0–18.0DeprecatediPadOS 15.0–18.0DeprecatedMac Catalyst 15.0–18.0DeprecatedmacOS 12.0–15.0DeprecatedtvOS 15.0–18.0DeprecatedvisionOS 1.0+watchOS 8.0–11.0Deprecated

``` source
func format(_ value: Date) -> AttributedString
```

Deprecated

Use Date.FormatStyle.Attributed or Date.VerbatimFormatStyle.Attributed instead

## Parameters 

`value`  

The date to format.

## Return Value

An attributed string representation of the date.

## Discussion

The `Date/ISO8601FormatStyle/format(_:)` instance method generates an attributed string from the provided date. Once you create a style, you can use it to format dates multiple times.

For an example of formatting multiple dates into plain strings, see `Date/FormatStyle/format(_:)`.

