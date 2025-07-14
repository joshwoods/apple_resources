

- os
- OSLogFloatFormatting
-  exponential 

Type Property

# exponential

The standard exponential format option.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
static var exponential: OSLogFloatFormatting { get }
```

## Mentioned in 

Generating Log Messages from Your Code

## Discussion

This option is equivalent to the `%e` option in `fprintf`. It prints the number in the form `[-]d.ddde±dd`, with `d` representing the digits of the number. The number of digits after the radix point is system-specific.

## See Also

### Getting the Standard Formats

static var fixed: OSLogFloatFormatting

The standard fixed-point format option.

static var hex: OSLogFloatFormatting

The standard hexadecimal format for floating-point values.

static var hybrid: OSLogFloatFormatting

A hybrid option that changes the format according to the size of the number.

