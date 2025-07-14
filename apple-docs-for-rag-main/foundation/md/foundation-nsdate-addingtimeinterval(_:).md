

- Foundation
- NSDate
-  addingTimeInterval(\_:) 

Instance Method

# addingTimeInterval(\_:)

Returns a new date object that is set to a given number of seconds relative to the receiver.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func addingTimeInterval(_ ti: TimeInterval) -> Self
```

## Parameters 

`ti`  

The number of seconds to add to the receiver. Use a negative value for seconds to have the returned object specify a date before the receiver.

## Return Value

A new `NSDate` object that is set to `seconds` seconds relative to the receiver. The date returned might have a representation different from the receiver’s.

## See Also

### Related Documentation

convenience init(timeInterval: TimeInterval, sinceDate: Date)

Returns a date object initialized relative to another given date by a given number of seconds.

func timeIntervalSince(Date) -> TimeInterval

Returns the interval between the receiver and another given date.

