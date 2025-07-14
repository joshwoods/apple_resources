

- Foundation
- FormatStyle
-  reference(to:allowedFields:maxFieldCount:thresholdField:) 

Type Method

# reference(to:allowedFields:maxFieldCount:thresholdField:)

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
static func reference(
    to date: Date,
    allowedFields: Set = [.year, .month, .day, .hour, .minute],
    maxFieldCount: Int = 2,
    thresholdField: Date.RelativeFormatStyle.Field = .day
) -> SystemFormatStyle.DateReference
```

Available when `Self` is `SystemFormatStyle.DateReference`.

