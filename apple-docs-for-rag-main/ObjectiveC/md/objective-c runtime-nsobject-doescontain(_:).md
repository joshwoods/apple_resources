

- Objective-C Runtime
- NSObject
-  doesContain(\_:) 

Instance Method

# doesContain(\_:)

Returns a Boolean value that indicates whether the receiver contains a given object.

Mac CatalystmacOS

``` source
func doesContain(_ object: Any) -> Bool
```

## Parameters 

`object`  

The object to search for in the receiver.

## Return Value

YES if the receiver contains `object`, otherwise NO.

## Discussion

Currently, doesContain(_:) messages are never sent to any object from within Cocoa itself.

The default implementation for this method provided by `NSObject` returns YES if the receiver is actually an `NSArray` object and an indexOfObjectIdentical(to:) message sent to the same object would return something other than `NSNotFound`.

