

- Objective-C Runtime
- NSObject
-  isCaseInsensitiveLike(\_:) 

Instance Method

# isCaseInsensitiveLike(\_:)

Returns a Boolean value that indicates whether receiver is considered to be “like” a given string when the case of characters in the receiver is ignored.

Mac CatalystmacOS

``` source
func isCaseInsensitiveLike(_ object: String) -> Bool
```

## Parameters 

`object`  

The string with which to compare the receiver.

## Return Value

YES if the receiver is considered to be “like” `aString` when the case of characters in the receiver is ignored, otherwise NO.

## Discussion

Currently, isCaseInsensitiveLike(_:) messages are never sent to any object from within Cocoa itself.

The default implementation for this method provided by `NSObject` returns NO. `NSString` also provides an implementation of this method, which returns YES if the receiver matches a pattern described by `aString`, ignoring the case of the characters in the receiver.

