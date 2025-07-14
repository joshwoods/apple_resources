

- Foundation
- NSOrderedSet
-  intersects(\_:) 

Instance Method

# intersects(\_:)

Returns a Boolean value that indicates whether at least one object in the receiving ordered set is also present in another given ordered set.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func intersects(_ other: NSOrderedSet) -> Bool
```

## Parameters 

`other`  

The other ordered set.

## Return Value

true if at least one object in the receiving ordered set is also present in `other`, otherwise false.

## See Also

### Comparing Sets

func isEqual(to: NSOrderedSet) -> Bool

Compares the receiving ordered set to another ordered set.

func intersectsSet(Set&lt;AnyHashable>) -> Bool

Returns a Boolean value that indicates whether at least one object in the receiving ordered set is also present in another given set.

func isSubset(of: NSOrderedSet) -> Bool

Returns a Boolean value that indicates whether every object in the receiving ordered set is also present in another given ordered set.

func isSubset(of: Set&lt;AnyHashable>) -> Bool

Returns a Boolean value that indicates whether every object in the receiving ordered set is also present in another given set.

