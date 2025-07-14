

- Foundation
- NSMutableSet
-  remove(\_:) 

Instance Method

# remove(\_:)

Removes a given object from the set.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func remove(_ object: Any)
```

## Parameters 

`object`  

The object to remove from the set.

## See Also

### Related Documentation

func minus(Set&lt;AnyHashable>)

Removes each object in another given set from the receiving set, if present.

func intersect(Set&lt;AnyHashable>)

Removes from the receiving set each object that isn’t a member of another given set.

### Adding and removing entries

func add(Any)

Adds a given object to the set, if it is not already a member.

func filter(using: NSPredicate)

Evaluates a given predicate against the set’s content and removes from the set those objects for which the predicate returns false.

func removeAllObjects()

Empties the set of all of its members.

func addObjects(from: [Any])

Adds to the set each object contained in a given array that is not already a member.

