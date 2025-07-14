

- Foundation
- Date
- Date.ISO8601FormatStyle
-  init(dateSeparator:dateTimeSeparator:timeZone:) 

Initializer

# init(dateSeparator:dateTimeSeparator:timeZone:)

Creates an instance using the provided date separator, date and time components separator, and time zone.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(
    dateSeparator: Date.ISO8601FormatStyle.DateSeparator = .dash,
    dateTimeSeparator: Date.ISO8601FormatStyle.DateTimeSeparator = .standard,
    timeZone: TimeZone = TimeZone(secondsFromGMT: 0)!
)
```

## Parameters 

`dateSeparator`  

The separator character used between the year, month, and day.

`dateTimeSeparator`  

The separator character used between the date and time components.

`timeZone`  

The TimeZone used to create the string representation of the date.

## Discussion

Possible values of `dateSeparator` are `dash` and `omitted`. Omitted is the default.

Possible values of `dateTimeSeparator` are `space` and `standard`. Standard is the default.

The following example shows the initizializer called with a variety of input parameters.

```
let aDate = Date()
print(aDate) // 2021-06-22 17:21:32 +0000
print(aDate.formatted(Date.ISO8601FormatStyle(dateSeparator: .omitted, dateTimeSeparator: .standard)))
// 20210622T172132Z

let cstDate = Date()
if let centralStandardTimeZone = TimeZone(identifier: "CST") {
   print(cstDate.formatted(Date.ISO8601FormatStyle(dateSeparator: .dash, dateTimeSeparator: .space, timeZone: centralStandardTimeZone)))
}
// 2021-06-22 122132-0500
```

