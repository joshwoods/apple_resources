

- Swift
- SetAlgebra
-  contains(\_:) 

Instance Method

# contains(\_:)

Returns a Boolean value that indicates whether the given element exists in the set.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func contains(_ member: Self.Element) -> Bool
```

**Required** Default implementation provided.

## Parameters 

`member`  

An element to look for in the set.

## Return Value

`true` if `member` exists in the set; otherwise, `false`.

## Discussion

This example uses the `contains(_:)` method to test whether an integer is a member of a set of prime numbers.

```
let primes: Set = [2, 3, 5, 7, 11, 13, 17, 19, 23, 29, 31, 37]
let x = 5
if primes.contains(x) {
    print("\(x) is prime!")
} else {
    print("\(x). Not prime.")
}
// Prints "5 is prime!"
```

## Default Implementations

### SetAlgebra Implementations

func contains(Self) -> Bool

Returns a Boolean value that indicates whether a given element is a member of the option set.

## See Also

### Testing for Membership

associatedtype Element

A type for which the conforming type provides a containment test.

**Required**

