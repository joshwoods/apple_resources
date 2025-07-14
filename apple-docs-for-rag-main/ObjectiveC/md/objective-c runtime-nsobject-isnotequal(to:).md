

- Objective-C Runtime
- NSObject
-  isNotEqual(to:) 

Instance Method

# isNotEqual(to:)

Returns a Boolean value that indicates whether the receiver is not equal to another given object.

Mac CatalystmacOS

``` source
func isNotEqual(to object: Any?) -> Bool
```

## Parameters 

`object`  

The object with which to compare the receiver.

## Return Value

YES if the receiver is not equal to `object`, otherwise NO.

## Discussion

Currently, isNotEqual(to:) messages are never sent to any object from within Cocoa itself.

The default implementation for this method provided by `NSObject` method returns YES if an `isEqual:` message sent to the same object would return NO.

