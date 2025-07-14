

- os
- OSLogInterpolation
-  appendInterpolation(\_:align:privacy:) 

Instance Method

# appendInterpolation(\_:align:privacy:)

Appends an interpolated string.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
mutating func appendInterpolation(
    _ argumentString: @autoclosure @escaping () -> String,
    align: OSLogStringAlignment = .none,
    privacy: OSLogPrivacy = .auto
)
```

## Parameters 

`argumentString`  

The interpolated string value to add to the message.

`align`  

The alignment to apply to the string. Use this parameter to specify the width of the column that contains the data, and the alignment of the data within that column. If you don’t specify this parameter, the system doesn’t align the value.

`privacy`  

The privacy level of the information. If you don’t specify this parameter, the default rules redact the string’s value.

## Discussion

Don’t call this function directly. The system calls it automatically when interpolating values of this type. When specifying the value in your string, you may include any of the indicated parameters to change the default presentation of that value.

## See Also

### Appending Strings

func appendInterpolation(@autoclosure () -> String, align: OSLogStringAlignment, privacy: OSLogPrivacy, attributes: String)

Appends an interpolated string with the specified attributes.

