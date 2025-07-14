

- SwiftData
- PersistentIdentifier
-  \

Operator

# \

Returns a Boolean value indicating whether the value of the first argument is less than that of the second argument.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static func  Bool
```

## Parameters 

`lhs`  

A value to compare.

`rhs`  

Another value to compare.

## Discussion

This function is the only requirement of the `Comparable` protocol. The remainder of the relational operator functions are implemented by the standard library for any type that conforms to `Comparable`.

## See Also

### Comparing identifiers

static func == (PersistentIdentifier, PersistentIdentifier) -> Bool

Returns a Boolean value indicating whether two values are equal.

