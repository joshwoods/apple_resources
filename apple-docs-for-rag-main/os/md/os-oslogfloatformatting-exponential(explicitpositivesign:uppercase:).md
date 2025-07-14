

- os
- OSLogFloatFormatting
-  exponential(explicitPositiveSign:uppercase:) 

Type Method

# exponential(explicitPositiveSign:uppercase:)

Creates a custom exponential format with a system-determined precision value.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
static func exponential(
    explicitPositiveSign: Bool = false,
    uppercase: Bool = false
) -> OSLogFloatFormatting
```

## Parameters 

`explicitPositiveSign`  

A Boolean value that indicates whether to display a plus (`+`) sign in front of positive numbers.

`uppercase`  

A Boolean value that indicates whether to uppercase letters that are part of the floating-point number. For example, it determines the capitalization of the exponent indicator `e` in the number `1.0e9`, or the letters in special values such as `NaN` and `Inf`.

## Return Value

A custom exponential format for floating-point numbers.

## See Also

### Creating a Custom Formatting Object

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

