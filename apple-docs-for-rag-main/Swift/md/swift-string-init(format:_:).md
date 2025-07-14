

- Swift
- String
-  init(format:\_:) 

Initializer

# init(format:\_:)

Returns a `String` object initialized by using a given format string as a template into which the remaining argument values are substituted.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    format: String,
    _ arguments: any CVarArg...
)
```

## See Also

### Creating a String Using Formats

init(format: String, arguments: [any CVarArg])

Returns a `String` object initialized by using a given format string as a template into which the remaining argument values are substituted according to the user’s default locale.

init(format: String, locale: Locale?, any CVarArg...)

Returns a `String` object initialized by using a given format string as a template into which the remaining argument values are substituted according to given locale information.

init(format: String, locale: Locale?, arguments: [any CVarArg])

Returns a `String` object initialized by using a given format string as a template into which the remaining argument values are substituted according to given locale information.

static func localizedStringWithFormat(String, any CVarArg...) -> String

Returns a string created by using a given format string as a template into which the remaining argument values are substituted according to the user’s default locale.

