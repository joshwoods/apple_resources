

- Objective-C Runtime
- NSObject
-  isLessThanOrEqual(to:) 

Instance Method

# isLessThanOrEqual(to:)

Returns a Boolean value that indicates whether the receiver is less than or equal to another given object.

Mac CatalystmacOS

``` source
func isLessThanOrEqual(to object: Any?) -> Bool
```

## Parameters 

`object`  

The object with which to compare the receiver.

## Return Value

YES if the receiver is less than or equal to `object`, otherwise NO.

## Discussion

During the evaluation of an `NSWhoseSpecifier` object that contains a test whose operator is `NSLessThanOrEqualToComparison`, an isLessThanOrEqual(to:) message may be sent to each potentially specified object, if the potentially specified object does not implement a scriptingIsLessThanOrEqual(to:) method and the object being tested against does not implement a scriptingIsGreaterThan(_:) method.

The default implementation for this method provided by `NSObject` method returns YES if a `compare:` message sent to the same object would return `NSOrderedAscending` or `NSOrderedSame`.

