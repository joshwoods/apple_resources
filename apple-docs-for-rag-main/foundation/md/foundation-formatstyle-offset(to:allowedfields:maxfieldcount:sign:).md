

- Foundation
- FormatStyle
-  offset(to:allowedFields:maxFieldCount:sign:) 

Type Method

# offset(to:allowedFields:maxFieldCount:sign:)

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
static func offset(
    to anchor: Date,
    allowedFields: Set = [.year, .month, .day, .hour, .minute, .second],
    maxFieldCount: Int = 2,
    sign: NumberFormatStyleConfiguration.SignDisplayStrategy = .automatic
) -> SystemFormatStyle.DateOffset
```

Available when `Self` is `SystemFormatStyle.DateOffset`.

