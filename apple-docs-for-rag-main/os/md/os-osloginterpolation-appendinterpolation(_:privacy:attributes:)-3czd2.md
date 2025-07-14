

- os
- OSLogInterpolation
-  appendInterpolation(\_:privacy:attributes:) 

Instance Method

# appendInterpolation(\_:privacy:attributes:)

Appends an interpolated object description with the specified attributes.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
mutating func appendInterpolation(
    _ argumentObject: @autoclosure @escaping () -> NSObject,
    privacy: OSLogPrivacy = .auto,
    attributes: String
)
```

## Parameters 

`argumentObject`  

The interpolated object, which the system automatically wraps in a closure. The object itself doesn’t appear in the log message. Instead, the system calls the object’s description method and incorporates the value it returns.

`privacy`  

The privacy level of the interpolated value, which the system applies when it renders the value in a log message. For more information, see OSLogPrivacy. The default value is auto.

`attributes`  

Additional information about the interpolated value. Tools that process log messages interpret these attributes, which you typically provide as key-value pairs. For example, Instruments processes any e_ngineering types\_ you embed in this value. For more information, see Instruments Developer Help.

## Discussion

Important

You don’t call this method directly. Instead, the framework calls it automatically when you append an interpolated object description to a log message.

## See Also

### Appending Objects

func appendInterpolation(@autoclosure () -> NSObject, privacy: OSLogPrivacy)

Appends an interpolated object description.

