

- Objective-C Runtime
- NSObject
-  isLike(\_:) 

Instance Method

# isLike(\_:)

Returns a Boolean value that indicates whether the receiver is “like” another given object.

Mac CatalystmacOS

``` source
func isLike(_ object: String) -> Bool
```

## Parameters 

`object`  

The object with which to compare the receiver.

## Return Value

YES if the receiver is considered to be “like” `object`, otherwise NO.

## Discussion

Currently, isLike(_:) messages are never sent to any object from within Cocoa itself.

The default implementation for this method provided by `NSObject` method returns NO. `NSString` also provides an implementation of this method, which returns YES if the receiver matches a pattern described by `object`.

