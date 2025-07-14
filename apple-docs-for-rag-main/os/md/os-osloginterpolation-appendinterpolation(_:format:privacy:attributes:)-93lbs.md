

- os
- OSLogInterpolation
-  appendInterpolation(\_:format:privacy:attributes:) 

Instance Method

# appendInterpolation(\_:format:privacy:attributes:)

Appends an interpolated collection of raw bytes with the specified attributes.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
mutating func appendInterpolation(
    _ pointer: @autoclosure @escaping () -> UnsafeRawBufferPointer,
    format: OSLogPointerFormat = .none,
    privacy: OSLogPrivacy = .auto,
    attributes: String
)
```

## Parameters 

`pointer`  

The interpolated collection of raw bytes. The system automatically wraps this value in a closure.

`format`  

The format to apply to the value when the system renders it in a log message. For more information, see OSLogPointerFormat. The default value is OSLogPointerFormat.none.

`privacy`  

The privacy level of the value, which the system applies when it renders the value in a log message. For more information, see OSLogPrivacy. The default value is auto.

`attributes`  

Additional information about the value. Tools that process log messages interpret these attributes, which you typically provide as key-value pairs. For example, Instruments processes any e_ngineering types\_ you embed in this value. For more information, see Instruments Developer Help.

## Discussion

Important

You don’t call this method directly. Instead, the framework calls it automatically when you append an interpolated collection of raw bytes to a log message.

## See Also

### Appending Pointer Data

func appendInterpolation(@autoclosure () -> UnsafeRawPointer, bytes: @autoclosure () -> Int, format: OSLogPointerFormat, privacy: OSLogPrivacy)

Appends interpolated pointer data.

func appendInterpolation(@autoclosure () -> UnsafeRawPointer, bytes: @autoclosure () -> Int, format: OSLogPointerFormat, privacy: OSLogPrivacy, attributes: String)

Appends interpolated pointer data with the specified attributes.

func appendInterpolation(@autoclosure () -> UnsafeRawBufferPointer, format: OSLogPointerFormat, privacy: OSLogPrivacy)

Appends an interpolated collection of raw bytes.

