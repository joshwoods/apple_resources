

- Foundation
- Date
- 
  - Date
- Date.FormatStyle
- Date.FormatStyle.Symbol
- Date.FormatStyle.Symbol.DayPeriod
-  with12s(\_:) 

Type Method

# with12s(\_:)

Static factory method that creates a custom day period format style using a style that represents midday and midnight.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func with12s(_ width: Date.FormatStyle.Symbol.DayPeriod.Width) -> Date.FormatStyle.Symbol.DayPeriod
```

## Parameters 

`width`  

Specifies the width of the string result.

## Return Value

A day period format style appropriate for the locale and specified width.

## See Also

### Modifying a Day Period

static func conversational(Date.FormatStyle.Symbol.DayPeriod.Width) -> Date.FormatStyle.Symbol.DayPeriod

Static factory method that creates a custom day period format style using a conversational style.

static func standard(Date.FormatStyle.Symbol.DayPeriod.Width) -> Date.FormatStyle.Symbol.DayPeriod

Static factory method that creates a custom day period format style using a standard style.

