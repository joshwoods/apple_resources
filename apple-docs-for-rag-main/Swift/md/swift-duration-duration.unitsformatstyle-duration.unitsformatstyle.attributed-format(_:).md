

- Swift
- Duration
- Duration.UnitsFormatStyle
- Duration.UnitsFormatStyle.Attributed
-  format(\_:) 

Instance Method

# format(\_:)

Creates a locale-aware attributed string representation from a duration value.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func format(_ duration: Duration) -> AttributedString
```

## Parameters 

`duration`  

The duration value to format.

## Return Value

A string representation of the duration, according to the style’s pattern and locale.

## Discussion

Use this method when you want to create a format style and repeatedly use it to format different durations. For one-off cases with default formatting, call the formatted() method of Duration instead.

