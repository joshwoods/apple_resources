

- os
- OSLogIntegerFormatting
-  octal(explicitPositiveSign:includePrefix:uppercase:minDigits:) 

Type Method

# octal(explicitPositiveSign:includePrefix:uppercase:minDigits:)

Creates a custom octal format that includes a minimum number of digits.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
static func octal(
    explicitPositiveSign: Bool = false,
    includePrefix: Bool = false,
    uppercase: Bool = false,
    minDigits: @autoclosure @escaping () -> Int
) -> OSLogIntegerFormatting
```

## Parameters 

`explicitPositiveSign`  

A Boolean value that indicates whether to display a plus (`+`) sign in front of positive integers.

`includePrefix`  

A Boolean that indicates whether to include a leading `0o` for octal numbers.

`uppercase`  

A Boolean value that indicates whether to uppercase numerals that are greater than 9.

`minDigits`  

The minimum number of digits to display for the octal value. If the number of digits in the octal number is less than this value, the logging system adds leading zeros.

## Return Value

A custom octal format for integers.

## See Also

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

