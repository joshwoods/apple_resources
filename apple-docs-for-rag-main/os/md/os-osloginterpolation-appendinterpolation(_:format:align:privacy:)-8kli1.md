

- os
- OSLogInterpolation
-  appendInterpolation(\_:format:align:privacy:) 

Instance Method

# appendInterpolation(\_:format:align:privacy:)

Appends an interpolated integer.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
mutating func appendInterpolation(
    _ number: @autoclosure @escaping () -> Int,
    format: OSLogIntegerFormatting = .decimal,
    align: OSLogStringAlignment = .none,
    privacy: OSLogPrivacy = .auto
)
```

## Parameters 

`number`  

The integer value to add to the message.

`format`  

The format to apply to the integer value. You format integers as decimal, hexadecimal, or octal values. If you don’t specify this parameter, the default format uses a decimal value. For more information, see OSLogIntegerFormatting.

`align`  

The alignment to apply to the value. Use this parameter to specify the width of the column containing the data, and the alignment of the data within that column. If you don’t specify this parameter, the system doesn’t align the value.

`privacy`  

The privacy level of the information. If you don’t specify this parameter, the system uses the default rules to determine whether to show the information.

## Discussion

Don’t call this function directly. The system calls it automatically when interpolating values of this type. When specifying the value in your string, you may include any of the indicated parameters to change the default presentation of that value.

## See Also

### Appending Signed Integers

func appendInterpolation(@autoclosure () -> Int8, format: OSLogIntegerFormatting, align: OSLogStringAlignment, privacy: OSLogPrivacy)

Appends an interpolated 8-bit integer.

func appendInterpolation(@autoclosure () -> Int16, format: OSLogIntegerFormatting, align: OSLogStringAlignment, privacy: OSLogPrivacy)

Appends an interpolated 16-bit integer.

func appendInterpolation(@autoclosure () -> Int32, format: OSLogInt32ExtendedFormat, privacy: OSLogPrivacy)

Appends an interpolated 32-bit integer.

func appendInterpolation(@autoclosure () -> Int32, format: OSLogInt32ExtendedFormat, privacy: OSLogPrivacy, attributes: String)

Appends an interpolated 32-bit integer with the specified attributes.

func appendInterpolation(@autoclosure () -> Int32, format: OSLogIntegerFormatting, align: OSLogStringAlignment, privacy: OSLogPrivacy)

Appends an interpolated 32-bit integer with the specified alignment.

func appendInterpolation(@autoclosure () -> Int64, format: OSLogIntegerFormatting, align: OSLogStringAlignment, privacy: OSLogPrivacy)

Appends an interpolated 64-bit integer.

