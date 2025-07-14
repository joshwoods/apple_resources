

- os
- OSLogInterpolation
-  appendInterpolation(\_:privacy:) 

Instance Method

# appendInterpolation(\_:privacy:)

Appends an interpolated object description.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
mutating func appendInterpolation(
    _ argumentObject: @autoclosure @escaping () -> NSObject,
    privacy: OSLogPrivacy = .auto
)
```

## Parameters 

`argumentObject`  

The object with the description you want to add to the message. This function calls the description method of the object and incorporates that value into the message string.

`privacy`  

The privacy level of the information. If you don’t specify this parameter, the default rules redact the object description.

## Discussion

Don’t call this function directly. The system calls it automatically when interpolating values of this type. When specifying the value in your string, you may include any of the indicated parameters to change the default presentation of that value.

## See Also

### Appending Objects

func appendInterpolation(@autoclosure () -> NSObject, privacy: OSLogPrivacy, attributes: String)

Appends an interpolated object description with the specified attributes.

