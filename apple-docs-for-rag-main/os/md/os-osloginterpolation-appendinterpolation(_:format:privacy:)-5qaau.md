

- os
- OSLogInterpolation
-  appendInterpolation(\_:format:privacy:) 

Instance Method

# appendInterpolation(\_:format:privacy:)

Appends an interpolated collection of raw bytes.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
mutating func appendInterpolation(
    _ pointer: @autoclosure @escaping () -> UnsafeRawBufferPointer,
    format: OSLogPointerFormat = .none,
    privacy: OSLogPrivacy = .auto
)
```

## Parameters 

`pointer`  

A pointer to data with an implicit size.

`format`  

The format to apply to the pointer. You format pointers as one of several different options. If you don’t specify this parameter, the system doesn’t format the value. For more information, see OSLogPointerFormat.

`privacy`  

The privacy level of the information. If you don’t specify this parameter, the system uses the default rules to determine whether to show the information.

## Discussion

Don’t call this function directly. The system calls it automatically when interpolating values of this type. When specifying the value in your string, you may include any of the indicated parameters to change the default presentation of that value.

## See Also

### Appending Pointer Data

func appendInterpolation(@autoclosure () -> UnsafeRawPointer, bytes: @autoclosure () -> Int, format: OSLogPointerFormat, privacy: OSLogPrivacy)

Appends interpolated pointer data.

func appendInterpolation(@autoclosure () -> UnsafeRawPointer, bytes: @autoclosure () -> Int, format: OSLogPointerFormat, privacy: OSLogPrivacy, attributes: String)

Appends interpolated pointer data with the specified attributes.

func appendInterpolation(@autoclosure () -> UnsafeRawBufferPointer, format: OSLogPointerFormat, privacy: OSLogPrivacy, attributes: String)

Appends an interpolated collection of raw bytes with the specified attributes.

