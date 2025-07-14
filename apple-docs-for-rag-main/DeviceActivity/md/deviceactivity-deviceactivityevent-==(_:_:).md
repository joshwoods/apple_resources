

- DeviceActivity
- DeviceActivityEvent
-  ==(\_:\_:) 

Operator

# ==(\_:\_:)

Returns a Boolean value indicating whether two values are equal.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
static func == (a: DeviceActivityEvent, b: DeviceActivityEvent) -> Bool
```

## Parameters 

`lhs`  

A value to compare.

`rhs`  

Another value to compare.

## Discussion

Equality is the inverse of inequality. For any values `a` and `b`, `a == b` implies that `a != b` is `false`.

## See Also

### Comparing Events and Schedules

static func != (Self, Self) -> Bool

Returns a Boolean value that indicates whether two values aren’t equal.

