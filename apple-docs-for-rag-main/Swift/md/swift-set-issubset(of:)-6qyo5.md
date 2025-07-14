

- Swift
- Set
-  isSubset(of:) 

Instance Method

# isSubset(of:)

Returns a Boolean value that indicates whether the set is a subset of the given sequence.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func isSubset(of possibleSuperset: S) -> Bool where Element == S.Element, S : Sequence
```

Available when `Element` conforms to `Hashable`.

## Parameters 

`possibleSuperset`  

A sequence of elements. `possibleSuperset` must be finite.

## Return Value

`true` if the set is a subset of `possibleSuperset`; otherwise, `false`.

## Discussion

Set *A* is a subset of another set *B* if every member of *A* is also a member of *B*.

```
let employees = ["Alicia", "Bethany", "Chris", "Diana", "Eric"]
let attendees: Set = ["Alicia", "Bethany", "Diana"]
print(attendees.isSubset(of: employees))
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

func isDisjoint&lt;S>(with: S) -> Bool

Returns a Boolean value that indicates whether the set has no members in common with the given sequence.

