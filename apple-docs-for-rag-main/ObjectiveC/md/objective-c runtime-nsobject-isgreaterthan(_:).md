

- Objective-C Runtime
- NSObject
-  isGreaterThan(\_:) 

Instance Method

# isGreaterThan(\_:)

Returns a Boolean value that indicates whether the receiver is greater than another given object.

Mac CatalystmacOS

``` source
func isGreaterThan(_ object: Any?) -> Bool
```

## Parameters 

`object`  

The object with which to compare the receiver.

## Return Value

YES if the receiver is greater than `object`, otherwise NO.

## Discussion

During the evaluation of an `NSWhoseSpecifier` object that contains a test whose operator is `NSGreaterThanComparison`, an isGreaterThan(_:) message may be sent to each potentially specified object, if the potentially specified object does not implement a scriptingIsGreaterThan(_:) method and the object being tested against does not implement a scriptingIsLessThanOrEqual(to:) method.

The default implementation for this method provided by `NSObject` returns YES if a `compare:` message sent to the same object would return `NSOrderedDescending`.

