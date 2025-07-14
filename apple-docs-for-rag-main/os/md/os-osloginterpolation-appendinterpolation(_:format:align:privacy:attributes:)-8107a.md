

- os
- OSLogInterpolation
-  appendInterpolation(\_:format:align:privacy:attributes:) 

Instance Method

# appendInterpolation(\_:format:align:privacy:attributes:)

Appends an interpolated numeric type using the specified attributes.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
mutating func appendInterpolation(
    _ number: @autoclosure @escaping () -> T,
    format: OSLogIntegerFormatting = .decimal,
    align: OSLogStringAlignment = .none,
    privacy: OSLogPrivacy = .auto,
    attributes: String
) where T : FixedWidthInteger
```

## Parameters 

`number`  

The interpolated numeric type, which the system automatically wraps in a closure. The type itself doesn’t appear in the log message. Instead, the system incorporates the type’s integer value.

`format`  

The format to apply to the value when the system renders it in a log message. For more information, see OSLogIntegerFormatting. The default value is decimal.

`align`  

The alignment and minimum number of columns to use when the system renders the value in a log message. For more information, see OSLogStringAlignment. The default value is none.

`privacy`  

The privacy level of the value, which the system applies when it renders the value in a log message. For more information, see OSLogPrivacy. The default value is auto.

`attributes`  

Additional information about the value. Tools that process log messages interpret these attributes, which you typically provide as key-value pairs. For example, Instruments processes any e_ngineering types\_ you embed in this value. For more information, see Instruments Developer Help.

## Discussion

Important

You don’t call this method directly. Instead, the framework calls it automatically when you append an interpolated type that adopts the FixedWidthInteger protocol to a log message.

## See Also

### Appending Generic Types

func appendInterpolation&lt;T>(@autoclosure () -> T, align: OSLogStringAlignment, privacy: OSLogPrivacy)

Appends an interpolated textual representation of a type.

func appendInterpolation&lt;T>(@autoclosure () -> T, align: OSLogStringAlignment, privacy: OSLogPrivacy, attributes: String)

Appends an interpolated textual representation of a type using the specified attributes.

func appendInterpolation(@autoclosure () -> any Any.Type, align: OSLogStringAlignment, privacy: OSLogPrivacy)

Appends an interpolated type description.

func appendInterpolation(@autoclosure () -> any Any.Type, align: OSLogStringAlignment, privacy: OSLogPrivacy, attributes: String)

Appends an interpolated type description with the specified attributes.

