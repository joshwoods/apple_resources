

- DeviceActivity
- DeviceActivityEvent
- DeviceActivityEvent.Name
-  !=(\_:\_:) 

Operator

# !=(\_:\_:)

Returns a Boolean value that indicates whether two values aren’t equal.

DeviceActivitySwiftiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
static func != (lhs: Self, rhs: Self) -> Bool
```

## Parameters 

`lhs`  

A value to compare.

`rhs`  

Another value to compare.

## Discussion

Inequality is the inverse of equality. For any values a and b, a != b implies that a == b is false. This is the default implementation of the not-equal-to operator (!=) for any type that conforms to Equatable.

## See Also

### Identifying and Comparing Errors

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

var hashValue: Int

The hash value.

