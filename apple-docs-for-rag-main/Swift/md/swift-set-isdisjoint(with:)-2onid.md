

- Swift
- Set
-  isDisjoint(with:) 

Instance Method

# isDisjoint(with:)

Returns a Boolean value that indicates whether the set has no members in common with the given sequence.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func isDisjoint(with other: S) -> Bool where Element == S.Element, S : Sequence
```

Available when `Element` conforms to `Hashable`.

## Parameters 

`other`  

A sequence of elements. `other` must be finite.

## Return Value

`true` if the set has no elements in common with `other`; otherwise, `false`.

## Discussion

In the following example, the `employees` set is disjoint with the elements of the `visitors` array because no name appears in both.

```
let employees: Set = ["Alicia", "Bethany", "Chris", "Diana", "Eric"]
let visitors = ["Marcia", "Nathaniel", "Olivia"]
print(employees.isDisjoint(with: visitors))
// Prints "true"
```

## See Also

### Comparing Sets

static func == (Set&lt;Element>, Set&lt;Element>) -> Bool

Returns a Boolean value indicating whether two sets have equal elements.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

func isSubset(of: Set&lt;Element>) -> Bool

Returns a Boolean value that indicates whether this set is a subset of the given set.

func isSubset&lt;S>(of: S) -> Bool

Returns a Boolean value that indicates whether the set is a subset of the given sequence.

func isStrictSubset(of: Set&lt;Element>) -> Bool

Returns a Boolean value that indicates whether the set is a strict subset of the given sequence.

func isStrictSubset&lt;S>(of: S) -> Bool

Returns a Boolean value that indicates whether the set is a strict subset of the given sequence.

func isSuperset(of: Set&lt;Element>) -> Bool

Returns a Boolean value that indicates whether this set is a superset of the given set.

func isSuperset&lt;S>(of: S) -> Bool

Returns a Boolean value that indicates whether the set is a superset of the given sequence.

func isStrictSuperset(of: Set&lt;Element>) -> Bool

Returns a Boolean value that indicates whether the set is a strict superset of the given sequence.

func isStrictSuperset&lt;S>(of: S) -> Bool

Returns a Boolean value that indicates whether the set is a strict superset of the given sequence.

func isDisjoint(with: Set&lt;Element>) -> Bool

Returns a Boolean value that indicates whether this set has no members in common with the given set.

