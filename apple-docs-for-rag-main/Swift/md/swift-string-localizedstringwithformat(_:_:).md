

- Swift
- String
-  localizedStringWithFormat(\_:\_:) 

Type Method

# localizedStringWithFormat(\_:\_:)

Returns a string created by using a given format string as a template into which the remaining argument values are substituted according to the user’s default locale.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static func localizedStringWithFormat(
    _ format: String,
    _ arguments: any CVarArg...
) -> String
```

## See Also

### Creating a String Using Formats

init(format: String, any CVarArg...)

Returns a `String` object initialized by using a given format string as a template into which the remaining argument values are substituted.

init(format: String, arguments: [any CVarArg])

Returns a `String` object initialized by using a given format string as a template into which the remaining argument values are substituted according to the user’s default locale.

init(format: String, locale: Locale?, any CVarArg...)

Returns a `String` object initialized by using a given format string as a template into which the remaining argument values are substituted according to given locale information.

init(format: String, locale: Locale?, arguments: [any CVarArg])

Returns a `String` object initialized by using a given format string as a template into which the remaining argument values are substituted according to given locale information.

