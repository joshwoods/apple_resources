

- Foundation
- IntegerFormatStyle
- IntegerFormatStyle.Percent
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

Use this method when you want to create a single style instance, and then use it to format multiple integers. To format a single integer, use the BinaryInteger instance method formatted(_:), passing in an instance of IntegerFormatStyle.Percent, or formatted() to use a default style.

