

- Foundation
- RelativeDateTimeFormatter
- RelativeDateTimeFormatter.DateTimeStyle
-  RelativeDateTimeFormatter.DateTimeStyle.named 

Case

# RelativeDateTimeFormatter.DateTimeStyle.named

A style that uses named styles to describe relative dates, such as “yesterday”, “last week”, or “next week”.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
case named
```

## Discussion

The formatter falls back to using RelativeDateTimeFormatter.DateTimeStyle.numeric if a name isn’t available.

## See Also

### Formatting Dates and Times

case numeric

A style that uses a numeric style to describe relative dates, such as “1 day ago” or “in 3 weeks”.

case numeric

A style that uses a numeric style to describe relative dates, such as “1 day ago” or “in 3 weeks”.

