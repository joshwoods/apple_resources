

- Foundation
- NSOrderedSet
-  isEqual(to:) 

Instance Method

# isEqual(to:)

Compares the receiving ordered set to another ordered set.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func isEqual(to other: NSOrderedSet) -> Bool
```

## Parameters 

`other`  

The ordered set with which to compare the receiving ordered set.

## Return Value

true if the contents of `other` are equal to the contents of the receiving ordered set, otherwise false.

## Discussion

Two ordered sets have equal contents if they each have the same number of members, if each member of one ordered set is present in the other, and the members are in the same order.

## See Also

### Related Documentation

func isEqual(_ object: Any?) -> Bool

Returns a Boolean value that indicates whether the receiver and a given object are equal.

### Comparing Sets

func intersects(NSOrderedSet) -> Bool

Returns a Boolean value that indicates whether at least one object in the receiving ordered set is also present in another given ordered set.

func intersectsSet(Set&lt;AnyHashable>) -> Bool

Returns a Boolean value that indicates whether at least one object in the receiving ordered set is also present in another given set.

func isSubset(of: NSOrderedSet) -> Bool

Returns a Boolean value that indicates whether every object in the receiving ordered set is also present in another given ordered set.

func isSubset(of: Set&lt;AnyHashable>) -> Bool

Returns a Boolean value that indicates whether every object in the receiving ordered set is also present in another given set.

