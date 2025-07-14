

- os
- OSLogInterpolation
-  appendInterpolation(\_:format:align:privacy:) 

Instance Method

# appendInterpolation(\_:format:align:privacy:)

Appends an interpolated float.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
mutating func appendInterpolation(
    _ number: @autoclosure @escaping () -> Float,
    format: OSLogFloatFormatting = .fixed,
    align: OSLogStringAlignment = .none,
    privacy: OSLogPrivacy = .auto
)
```

## Parameters 

`number`  

The float value to add to the message.

`format`  

The format to apply to the float value. You format floating-point numbers as fixed-point, hexadecimal, exponential, or hybrid values. If you don’t specify this parameter, the default format uses a fixed-point value. For more information, see OSLogFloatFormatting.

`align`  

The alignment to apply to the value. Use this parameter to specify the width of the column containing the data, and the alignment of the data within that column. If you don’t specify this parameter, the system doesn’t align the value.

`privacy`  

The privacy level of the information. If you don’t specify this parameter, the system uses the default rules to determine whether to show the information.

## Discussion

Don’t call this function directly. The system calls it automatically when interpolating values of this type. When specifying the value in your string, you may include any of the indicated parameters to change the default presentation of that value.

## See Also

### Appending Floats

func appendInterpolation(@autoclosure () -> Float, format: OSLogFloatFormatting, align: OSLogStringAlignment, privacy: OSLogPrivacy, attributes: String)

Appends an interpolated float with the specified attributes.

