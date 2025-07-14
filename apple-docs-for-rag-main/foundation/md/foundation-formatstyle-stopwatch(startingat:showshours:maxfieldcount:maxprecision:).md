

- Foundation
- FormatStyle
-  stopwatch(startingAt:showsHours:maxFieldCount:maxPrecision:) 

Type Method

# stopwatch(startingAt:showsHours:maxFieldCount:maxPrecision:)

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
static func stopwatch(
    startingAt startDate: Date,
    showsHours: Bool = true,
    maxFieldCount: Int = 4,
    maxPrecision: Duration = .milliseconds(10)
) -> SystemFormatStyle.Stopwatch
```

Available when `Self` is `SystemFormatStyle.Stopwatch`.

