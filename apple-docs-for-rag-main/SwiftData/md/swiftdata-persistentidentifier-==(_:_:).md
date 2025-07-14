

- SwiftData
- PersistentIdentifier
-  ==(\_:\_:) 

Operator

# ==(\_:\_:)

Returns a Boolean value indicating whether two values are equal.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static func == (lhs: PersistentIdentifier, rhs: PersistentIdentifier) -> Bool
```

## Parameters 

`lhs`  

A value to compare.

`rhs`  

Another value to compare.

## Discussion

Equality is the inverse of inequality. For any values `a` and `b`, `a == b` implies that `a != b` is `false`.

## See Also

### Comparing identifiers

static func &lt; (PersistentIdentifier, PersistentIdentifier) -> Bool

Returns a Boolean value indicating whether the value of the first argument is less than that of the second argument.

