

- os
- OSLogInterpolation
-  appendInterpolation(\_:format:privacy:) 

Instance Method

# appendInterpolation(\_:format:privacy:)

Adds a Boolean argument to the message.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
mutating func appendInterpolation(
    _ boolean: @autoclosure @escaping () -> Bool,
    format: OSLogBoolFormat = .truth,
    privacy: OSLogPrivacy = .auto
)
```

## Parameters 

`boolean`  

The Boolean value to add to the message.

`format`  

The format to apply to the Boolean value. You format Boolean values as either true/false or yes/no strings. If you don’t specify this parameter, the default format uses true/false strings. For more information, see OSLogBoolFormat.

`privacy`  

The privacy level of the information. If you don’t specify this parameter, the system uses the default rules to determine whether to show the information.

## Discussion

Don’t call this function directly. The system calls it automatically when interpolating values of this type. When specifying the value in your string, you may include any of the indicated parameters to change the default presentation of that value.

