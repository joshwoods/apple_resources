

- os
- OSLogFloatFormatting
-  fixed 

Type Property

# fixed

The standard fixed-point format option.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
static var fixed: OSLogFloatFormatting { get }
```

## Mentioned in 

Generating Log Messages from Your Code

## Discussion

This option is equivalent to the `%f` option of `fprintf`, which prints all digits before the radix point and a system-specific number of digits after the radix point.

## See Also

### Getting the Standard Formats

static var hex: OSLogFloatFormatting

The standard hexadecimal format for floating-point values.

static var exponential: OSLogFloatFormatting

The standard exponential format option.

static var hybrid: OSLogFloatFormatting

A hybrid option that changes the format according to the size of the number.

