

- Foundation
- Date
- Date.ParseStrategy
-  init(format:locale:timeZone:calendar:isLenient:twoDigitStartDate:) 

Initializer

# init(format:locale:timeZone:calendar:isLenient:twoDigitStartDate:)

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(
    format: Date.FormatString,
    locale: Locale? = nil,
    timeZone: TimeZone,
    calendar: Calendar = Calendar(identifier: .gregorian),
    isLenient: Bool = true,
    twoDigitStartDate: Date = Date(timeIntervalSince1970: 0)
)
```

