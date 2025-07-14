

- Foundation
- Date
- Date.ISO8601FormatStyle
-  init(dateSeparator:dateTimeSeparator:timeSeparator:timeZoneSeparator:includingFractionalSeconds:timeZone:) 

Initializer

# init(dateSeparator:dateTimeSeparator:timeSeparator:timeZoneSeparator:includingFractionalSeconds:timeZone:)

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(
    dateSeparator: Date.ISO8601FormatStyle.DateSeparator = .dash,
    dateTimeSeparator: Date.ISO8601FormatStyle.DateTimeSeparator = .standard,
    timeSeparator: Date.ISO8601FormatStyle.TimeSeparator = .colon,
    timeZoneSeparator: Date.ISO8601FormatStyle.TimeZoneSeparator = .omitted,
    includingFractionalSeconds: Bool = false,
    timeZone: TimeZone = TimeZone(secondsFromGMT: 0)!
)
```

