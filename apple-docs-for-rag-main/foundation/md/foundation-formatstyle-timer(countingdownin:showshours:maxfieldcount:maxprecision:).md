

- Foundation
- FormatStyle
-  timer(countingDownIn:showsHours:maxFieldCount:maxPrecision:) 

Type Method

# timer(countingDownIn:showsHours:maxFieldCount:maxPrecision:)

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
static func timer(
    countingDownIn interval: Range,
    showsHours: Bool = true,
    maxFieldCount: Int = 3,
    maxPrecision: Duration = .seconds(1)
) -> SystemFormatStyle.Timer
```

Available when `Self` is `SystemFormatStyle.Timer`.

