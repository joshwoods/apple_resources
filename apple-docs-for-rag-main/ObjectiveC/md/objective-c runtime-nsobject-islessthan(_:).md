

- Objective-C Runtime
- NSObject
-  isLessThan(\_:) 

Instance Method

# isLessThan(\_:)

Returns a Boolean value that indicates whether the receiver is less than another given object.

Mac CatalystmacOS

``` source
func isLessThan(_ object: Any?) -> Bool
```

## Parameters 

`object`  

The object with which to compare the receiver.

## Return Value

YES if the receiver is less than `object`, otherwise NO.

## Discussion

During the evaluation of an `NSWhoseSpecifier` object that contains a test whose operator is `NSLessThanComparison`, an isLessThan(_:) message may be sent to each potentially specified object, if the potentially specified object does not implement a scriptingIsLessThan(_:) method and the object being tested against does not implement a scriptingIsGreaterThanOrEqual(to:) method.

The default implementation for this method provided by `NSObject` method returns YES if a `compare:` message sent to the same object would return `NSOrderedAscending`.

