

- os
- OSLogIntegerFormatting
-  decimal(explicitPositiveSign:) 

Type Method

# decimal(explicitPositiveSign:)

Creates a decimal format with custom handling of the numerical sign.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
static func decimal(explicitPositiveSign: Bool = false) -> OSLogIntegerFormatting
```

## Parameters 

`explicitPositiveSign`  

A Boolean value that indicates whether to display a plus (`+`) sign in front of positive integers.

## Return Value

A custom decimal format for integers.

## See Also

### Creating a Custom Integer Format

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

