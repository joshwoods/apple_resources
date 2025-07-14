

- Foundation
- NSOrderedSet
-  isSubset(of:) 

Instance Method

# isSubset(of:)

Returns a Boolean value that indicates whether every object in the receiving ordered set is also present in another given set.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func isSubset(of set: Set) -> Bool
```

## Parameters 

`set`  

The set with which to compare the receiving ordered set.

## Return Value

true if every object in the receiving ordered set is also present in `set`, otherwise false.

## See Also

### Comparing Sets

func isEqual(to: NSOrderedSet) -> Bool

Compares the receiving ordered set to another ordered set.

func intersects(NSOrderedSet) -> Bool

Returns a Boolean value that indicates whether at least one object in the receiving ordered set is also present in another given ordered set.

func intersectsSet(Set&lt;AnyHashable>) -> Bool

Returns a Boolean value that indicates whether at least one object in the receiving ordered set is also present in another given set.

func isSubset(of: NSOrderedSet) -> Bool

Returns a Boolean value that indicates whether every object in the receiving ordered set is also present in another given ordered set.

