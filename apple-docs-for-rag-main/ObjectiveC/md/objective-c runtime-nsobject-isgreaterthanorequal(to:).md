

- Objective-C Runtime
- NSObject
-  isGreaterThanOrEqual(to:) 

Instance Method

# isGreaterThanOrEqual(to:)

Returns a Boolean value that indicates whether the receiver is greater than or equal to another given object.

Mac CatalystmacOS

``` source
func isGreaterThanOrEqual(to object: Any?) -> Bool
```

## Parameters 

`object`  

The object with which to compare the receiver.

## Return Value

YES if the receiver is greater than or equal to `object`, otherwise NO.

## Discussion

During the evaluation of an `NSWhoseSpecifier` object that contains a test whose operator is `NSGreaterThanOrEqualToComparison`, anisGreaterThanOrEqual(to:) message may be sent to each potentially specified object, if the potentially specified object does not implement a scriptingIsGreaterThanOrEqual(to:) method and the object being tested against does not implement a scriptingIsLessThan(_:) method.

The default implementation for this method provided by `NSObject` returns YES if a `compare:` message sent to the same object would return `NSOrderedSame` or `NSOrderedDescending`.

