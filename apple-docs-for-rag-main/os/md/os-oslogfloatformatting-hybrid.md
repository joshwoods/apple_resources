

- os
- OSLogFloatFormatting
-  hybrid 

Type Property

# hybrid

A hybrid option that changes the format according to the size of the number.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
static var hybrid: OSLogFloatFormatting { get }
```

## Mentioned in 

Generating Log Messages from Your Code

## Discussion

This option is equivalent to the `%g` option in `fprintf`. It behaves like the fixed option when the number is close to `1.0`, and like the exponential option when the number has a large exponent.

## See Also

### Getting the Standard Formats

static var fixed: OSLogFloatFormatting

The standard fixed-point format option.

static var hex: OSLogFloatFormatting

The standard hexadecimal format for floating-point values.

static var exponential: OSLogFloatFormatting

The standard exponential format option.

