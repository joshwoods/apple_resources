

- Foundation
- NSSet
-  isSubset(of:) 

Instance Method

# isSubset(of:)

Returns a Boolean value that indicates whether every object in the receiving set is also present in another given set.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func isSubset(of otherSet: Set) -> Bool
```

## Parameters 

`otherSet`  

The set with which to compare the receiving set.

## Return Value

true if every object in the receiving set is also present in `otherSet`, otherwise false.

## Discussion

Object equality is tested using isEqual:.

## See Also

### Comparing Sets

func intersects(Set&lt;AnyHashable>) -> Bool

Returns a Boolean value that indicates whether at least one object in the receiving set is also present in another given set.

func isEqual(to: Set&lt;AnyHashable>) -> Bool

Compares the receiving set to another set.

func value(forKey: String) -> Any

Return a set containing the results of invoking `valueForKey:` on each of the receiving set’s members.

func setValue(Any?, forKey: String)

Invokes `setValue:forKey:` on each of the set’s members.

