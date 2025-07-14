

- os
- OSLogInterpolation
-  appendInterpolation(\_:align:privacy:) 

Instance Method

# appendInterpolation(\_:align:privacy:)

Appends an interpolated textual representation of a type.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
mutating func appendInterpolation(
    _ value: @autoclosure @escaping () -> T,
    align: OSLogStringAlignment = .none,
    privacy: OSLogPrivacy = .auto
) where T : CustomStringConvertible
```

## Parameters 

`value`  

An item that conforms to the CustomStringConvertible protocol.

`align`  

The alignment to apply to the string. Use this parameter to specify the width of the column containing the data, and the alignment of the data within that column. If you don’t specify this parameter, the system doesn’t align the value.

`privacy`  

The privacy level of the information. If you don’t specify this parameter, the system uses the default rules to determine whether to show the information.

## Discussion

Don’t call this function directly. The system calls it automatically when interpolating values of this type. When specifying the value in your string, you may include any of the indicated parameters to change the default presentation of that value.

## See Also

### Appending Generic Types

func appendInterpolation&lt;T>(@autoclosure () -> T, align: OSLogStringAlignment, privacy: OSLogPrivacy, attributes: String)

Appends an interpolated textual representation of a type using the specified attributes.

func appendInterpolation&lt;T>(@autoclosure () -> T, format: OSLogIntegerFormatting, align: OSLogStringAlignment, privacy: OSLogPrivacy, attributes: String)

Appends an interpolated numeric type using the specified attributes.

func appendInterpolation(@autoclosure () -> any Any.Type, align: OSLogStringAlignment, privacy: OSLogPrivacy)

Appends an interpolated type description.

func appendInterpolation(@autoclosure () -> any Any.Type, align: OSLogStringAlignment, privacy: OSLogPrivacy, attributes: String)

Appends an interpolated type description with the specified attributes.

