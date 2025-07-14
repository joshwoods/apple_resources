

- App Intents
- TypeDisplayRepresentation
-  numericFormat 

Instance Property

# numericFormat

A string representing a count for the type, e.g. “2 books”.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var numericFormat: LocalizedStringResource?
```

## Discussion

In your `numericFormat` implementation, use `StringInterpolation` placeholders and provide a `.stringsdict` file with all possible pluralizations for the type, such as “0 books”, “1 book”, and “2 books”.

Example:

```
TypeDisplayRepresentation(
    name: LocalizedStringResource("Book"),
    numericFormat: LocalizedStringResource("\(placeholder: .int) books")
)
```

```

   Book

     NSStringLocalizedFormatKey
     %#@VARIABLE@
     VARIABLE

       NSStringFormatSpecTypeKey
       NSStringPluralRuleType
       one
       Book
       other
       Books

   %lld books

     NSStringLocalizedFormatKey
     %#@count@
     count

       NSStringFormatSpecTypeKey
       NSStringPluralRuleType
       NSStringFormatValueTypeKey
       lld
       zero
       %lld books
       one
       %lld book
       other
       %lld books

```

