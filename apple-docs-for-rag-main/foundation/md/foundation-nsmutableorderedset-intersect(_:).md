

- Foundation
- NSMutableOrderedSet
-  intersect(\_:) 

Instance Method

# intersect(\_:)

Removes from the receiving ordered set each object that isn’t a member of another ordered set.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func intersect(_ other: NSOrderedSet)
```

## Parameters 

`other`  

The ordered set with which to perform the intersection.

## See Also

### Combining and Recombining Entries

func intersectSet(Set&lt;AnyHashable>)

Removes from the receiving ordered set each object that isn’t a member of another set.

func minus(NSOrderedSet)

Removes each object in another given ordered set from the receiving mutable ordered set, if present.

func minusSet(Set&lt;AnyHashable>)

Removes each object in another given set from the receiving mutable ordered set, if present.

func union(NSOrderedSet)

Adds each object in another given ordered set to the receiving mutable ordered set, if not present.

func unionSet(Set&lt;AnyHashable>)

Adds each object in another given set to the receiving mutable ordered set, if not present.

