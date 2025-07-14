

- os
-  OSLogIntegerFormatting 

Structure

# OSLogIntegerFormatting

The formatting options for integer values.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
@frozen
struct OSLogIntegerFormatting
```

## Mentioned in 

Generating Log Messages from Your Code

## Overview

An OSLogIntegerFormatting structure encapsulates the formatting details for integer numbers. Use the static decimal, hex, and octal structures to apply default formatting to integer values. You can also create new OSLogIntegerFormatting structures that customize the rules for handling a leading plus sign, special numerical prefixes, the minimum number of digits, and more.

## Topics

### Getting the Standard Formats

static var decimal: OSLogIntegerFormatting

The standard decimal format option.

static var hex: OSLogIntegerFormatting

The standard hexadecimal format option.

static var octal: OSLogIntegerFormatting

The standard octal format option.

### Creating a Custom Integer Format

static func decimal(explicitPositiveSign: Bool) -> OSLogIntegerFormatting

Creates a decimal format with custom handling of the numerical sign.

static func decimal(explicitPositiveSign: Bool, minDigits: @autoclosure () -> Int) -> OSLogIntegerFormatting

Creates a decimal format with custom handling of the numerical sign and the minimum number of digits.

static func hex(explicitPositiveSign: Bool, includePrefix: Bool, uppercase: Bool) -> OSLogIntegerFormatting

Creates a custom hexidecimal format that displays the exact number of digits in the number.

static func hex(explicitPositiveSign: Bool, includePrefix: Bool, uppercase: Bool, minDigits: @autoclosure () -> Int) -> OSLogIntegerFormatting

Creates a custom hexidecimal format that includes a minimum number of digits.

static func octal(explicitPositiveSign: Bool, includePrefix: Bool, uppercase: Bool) -> OSLogIntegerFormatting

Creates a custom octal format that displays the exact number of digits in the number.

static func octal(explicitPositiveSign: Bool, includePrefix: Bool, uppercase: Bool, minDigits: @autoclosure () -> Int) -> OSLogIntegerFormatting

Creates a custom octal format that includes a minimum number of digits.

## See Also

### Value Formatters

enum OSLogBoolFormat

The formatting options for Boolean values.

enum OSLogInt32ExtendedFormat

The formatting options for 32-bit integer values.

struct OSLogFloatFormatting

The formatting options for double and floating-point numbers.

enum OSLogPointerFormat

The formatting options for pointer data.

