

- Foundation
- IntegerFormatStyle
-  format(\_:) 

Instance Method

# format(\_:)

Formats an integer, using this style.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func format(_ value: Value) -> String
```

Available when `Value` conforms to `BinaryInteger`.

## Parameters 

`value`  

The integer to format.

## Return Value

A string representation of `value`, formatted according to the style’s configuration.

## Discussion

Use this method when you want to create a single style instance and use it to format multiple integers. The following example creates a style that uses the `en_US` locale, and adds the compactName modifier. It applies this style to all the integers in an array.

```
let compactNameStyle = IntegerFormatStyle(
    locale: Locale(identifier: "en_US"))
    .notation(.compactName)
let nums = [100, 1000, 10000, 100000, 1000000]
let formattedNums = nums.map { compactNameStyle.format($0) } // ["100", "1K", "10K", "100K", "1M"]

```

To format a single integer, use the BinaryInteger instance method formatted(_:), passing in an instance of IntegerFormatStyle, or formatted() to use a default style.

