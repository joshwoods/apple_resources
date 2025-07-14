

- os
- OSLogInterpolation
-  appendInterpolation(\_:format:align:privacy:) 

Instance Method

# appendInterpolation(\_:format:align:privacy:)

Appends an interpolated unsigned 8-bit integer.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
mutating func appendInterpolation(
    _ number: @autoclosure @escaping () -> UInt8,
    format: OSLogIntegerFormatting = .decimal,
    align: OSLogStringAlignment = .none,
    privacy: OSLogPrivacy = .auto
)
```

## Parameters 

`number`  

The unsigned 8-bit integer value to add to the message.

`format`  

The format to apply to the integer value. You format integers as decimal, hexadecimal, or octal values. If you don’t specify this parameter, the default format uses a decimal value. For more information, see OSLogIntegerFormatting.

`align`  

The alignment to apply to the value. Use this parameter to specify the width of the column containing the data, and the alignment of the data within that column. If you don’t specify this parameter, the system doesn’t align the value.

`privacy`  

The privacy level of the information. If you don’t specify this parameter, the system uses the default rules to determine whether to show the information.

## Discussion

Don’t call this function directly. The system calls it automatically when interpolating values of this type. When specifying the value in your string, you may include any of the indicated parameters to change the default presentation of that value.

## See Also

### Appending Unsigned Integers

func appendInterpolation(@autoclosure () -> UInt, format: OSLogIntegerFormatting, align: OSLogStringAlignment, privacy: OSLogPrivacy)

Appends an interpolated unsigned integer.

func appendInterpolation(@autoclosure () -> UInt16, format: OSLogIntegerFormatting, align: OSLogStringAlignment, privacy: OSLogPrivacy)

Appends an interpolated unsigned 16-bit integer.

func appendInterpolation(@autoclosure () -> UInt32, format: OSLogIntegerFormatting, align: OSLogStringAlignment, privacy: OSLogPrivacy)

Appends an interpolated unsigned 32-bit integer.

func appendInterpolation(@autoclosure () -> UInt64, format: OSLogIntegerFormatting, align: OSLogStringAlignment, privacy: OSLogPrivacy)

Appends an interpolated unsigned 64-bit integer.

