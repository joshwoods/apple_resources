

- Swift
- Set
-  contains(\_:) 

Instance Method

# contains(\_:)

Returns a Boolean value that indicates whether the given element exists in the set.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func contains(_ member: Element) -> Bool
```

Available when `Element` conforms to `Hashable`.

## Parameters 

`member`  

An element to look for in the set.

## Return Value

`true` if `member` exists in the set; otherwise, `false`.

## Discussion

This example uses the `contains(_:)` method to test whether an integer is a member of a set of prime numbers.

```
let primes: Set = [2, 3, 5, 7]
let x = 5
if primes.contains(x) {
    print("\(x) is prime!")
} else {
    print("\(x). Not prime.")
}
// Prints "5 is prime!"
```

Complexity

O(1)

