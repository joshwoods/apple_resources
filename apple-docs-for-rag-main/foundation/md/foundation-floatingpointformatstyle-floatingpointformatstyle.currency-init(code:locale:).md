

- Foundation
- FloatingPointFormatStyle
- FloatingPointFormatStyle.Currency
-  init(code:locale:) 

Initializer

# init(code:locale:)

Creates a floating-point currency format style that uses the given currency code and locale.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(
    code: String,
    locale: Locale = .autoupdatingCurrent
)
```

## Parameters 

`code`  

The currency code to use, such as `EUR` or `JPY`.

`locale`  

The locale to use when formatting or parsing floating-point values. Defaults to autoupdatingCurrent.

