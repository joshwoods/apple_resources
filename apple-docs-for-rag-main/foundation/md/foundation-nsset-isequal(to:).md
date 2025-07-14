

- Foundation
- NSSet
-  isEqual(to:) 

Instance Method

# isEqual(to:)

Compares the receiving set to another set.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func isEqual(to otherSet: Set) -> Bool
```

## Parameters 

`otherSet`  

The set with which to compare the receiving set.

## Return Value

true if the contents of `otherSet` are equal to the contents of the receiving set, otherwise false.

## Discussion

Two sets have equal contents if they each have the same number of members and if each member of one set is present in the other. Object equality is tested using isEqual:.

## See Also

### Related Documentation

func isEqual(_ object: Any?) -> Bool

Returns a Boolean value that indicates whether the receiver and a given object are equal.

### Comparing Sets

func isSubset(of: Set&lt;AnyHashable>) -> Bool

Returns a Boolean value that indicates whether every object in the receiving set is also present in another given set.

func intersects(Set&lt;AnyHashable>) -> Bool

Returns a Boolean value that indicates whether at least one object in the receiving set is also present in another given set.

func value(forKey: String) -> Any

Return a set containing the results of invoking `valueForKey:` on each of the receiving set’s members.

func setValue(Any?, forKey: String)

Invokes `setValue:forKey:` on each of the set’s members.

