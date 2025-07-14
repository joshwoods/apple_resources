

- os
- OSLogInterpolation
-  appendInterpolation(\_:format:align:privacy:attributes:) 

Instance Method

# appendInterpolation(\_:format:align:privacy:attributes:)

Appends an interpolated float with the specified attributes.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
mutating func appendInterpolation(
    _ number: @autoclosure @escaping () -> Float,
    format: OSLogFloatFormatting = .fixed,
    align: OSLogStringAlignment = .none,
    privacy: OSLogPrivacy = .auto,
    attributes: String
)
```

## Parameters 

`number`  

The interpolated float. The system automatically wraps this value in a closure.

`format`  

The format to apply to the value when the system renders it in a log message. For more information, see OSLogFloatFormatting. The default value is fixed.

`align`  

The alignment and minimum number of columns to use when the system renders the value in a log message. For more information, see OSLogStringAlignment. The default value is none.

`privacy`  

The privacy level of the value, which the system applies when it renders the value in a log message. For more information, see OSLogPrivacy. The default value is auto.

`attributes`  

Additional information about the value. Tools that process log messages interpret these attributes, which you typically provide as key-value pairs. For example, Instruments processes any e_ngineering types\_ you embed in this value. For more information, see Instruments Developer Help.

## Discussion

Important

You don’t call this method directly. Instead, the framework calls it automatically when you append an interpolated float to a log message.

## See Also

### Appending Floats

func appendInterpolation(@autoclosure () -> Float, format: OSLogFloatFormatting, align: OSLogStringAlignment, privacy: OSLogPrivacy)

Appends an interpolated float.

