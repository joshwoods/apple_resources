

- os
-  OSLogFloatFormatting 

Structure

# OSLogFloatFormatting

The formatting options for double and floating-point numbers.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
@frozen
struct OSLogFloatFormatting
```

## Mentioned in 

Generating Log Messages from Your Code

## Overview

An OSLogFloatFormatting structure encapsulates the formatting details for `double` and `float` values. Use the static fixed, hex, exponential, and hybrid structures to apply default formatting for floating-point values. You can also create new OSLogFloatFormatting structures that customize the rules for handling a leading plus sign, precision information, and more.

## Topics

### Getting the Standard Formats

static var fixed: OSLogFloatFormatting

The standard fixed-point format option.

static var hex: OSLogFloatFormatting

The standard hexadecimal format for floating-point values.

static var exponential: OSLogFloatFormatting

The standard exponential format option.

static var hybrid: OSLogFloatFormatting

A hybrid option that changes the format according to the size of the number.

### Creating a Custom Formatting Object

static func exponential(explicitPositiveSign: Bool, uppercase: Bool) -> OSLogFloatFormatting

Creates a custom exponential format with a system-determined precision value.

static func exponential(precision: @autoclosure () -> Int, explicitPositiveSign: Bool, uppercase: Bool) -> OSLogFloatFormatting

Creates a custom exponential format with the specified precision value.

static func fixed(explicitPositiveSign: Bool, uppercase: Bool) -> OSLogFloatFormatting

Creates a custom fixed-point format with a system-determined precision value.

static func fixed(precision: @autoclosure () -> Int, explicitPositiveSign: Bool, uppercase: Bool) -> OSLogFloatFormatting

Creates a custom fixed-point format with the specified precision value.

static func hex(explicitPositiveSign: Bool, uppercase: Bool) -> OSLogFloatFormatting

Creates a custom hexadecimal format.

static func hybrid(explicitPositiveSign: Bool, uppercase: Bool) -> OSLogFloatFormatting

Creates a custom hybrid format with a system-determined precision value.

static func hybrid(precision: @autoclosure () -> Int, explicitPositiveSign: Bool, uppercase: Bool) -> OSLogFloatFormatting

Creates a custom hybrid format with the precision value.

## See Also

### Value Formatters

enum OSLogBoolFormat

The formatting options for Boolean values.

struct OSLogIntegerFormatting

The formatting options for integer values.

enum OSLogInt32ExtendedFormat

The formatting options for 32-bit integer values.

enum OSLogPointerFormat

The formatting options for pointer data.

