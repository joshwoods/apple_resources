

- Objective-C Runtime
- NSObject
-  isEqual(to:) 

Instance Method

# isEqual(to:)

Returns a Boolean value that indicates whether the receiver is equal to another given object.

Mac CatalystmacOS

``` source
func isEqual(to object: Any?) -> Bool
```

## Parameters 

`object`  

The object with which to compare the receiver.

## Return Value

YES if the receiver is equal to `object`, otherwise NO. In effect returns NO if receiver is `nil`.

## Discussion

During the evaluation of an `NSWhoseSpecifier` object that contains a test whose operator is `NSEqualToComparison`, an isEqual(to:) message may be sent to each potentially specified object, if neither the potentially specified object nor the object being tested against implements a scriptingIsEqual(to:) method.

The default implementation for this method provided by `NSObject` returns YES if an `isEqualTo:` message sent to the same object would return YES.

