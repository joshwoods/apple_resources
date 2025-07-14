

- Foundation
- NSMutableOrderedSet
-  unionSet(\_:) 

Instance Method

# unionSet(\_:)

Adds each object in another given set to the receiving mutable ordered set, if not present.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func unionSet(_ other: Set)
```

## Parameters 

`other`  

The set of objects to add to the receiving mutable ordered set.

## See Also

### Combining and Recombining Entries

func intersect(NSOrderedSet)

Removes from the receiving ordered set each object that isn’t a member of another ordered set.

func intersectSet(Set&lt;AnyHashable>)

Removes from the receiving ordered set each object that isn’t a member of another set.

func minus(NSOrderedSet)

Removes each object in another given ordered set from the receiving mutable ordered set, if present.

func minusSet(Set&lt;AnyHashable>)

Removes each object in another given set from the receiving mutable ordered set, if present.

func union(NSOrderedSet)

Adds each object in another given ordered set to the receiving mutable ordered set, if not present.

