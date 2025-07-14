

- Foundation
- NSMutableSet
-  add(\_:) 

Instance Method

# add(\_:)

Adds a given object to the set, if it is not already a member.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func add(_ object: Any)
```

## Parameters 

`object`  

The object to add to the set.

## See Also

### Related Documentation

func union(Set&lt;AnyHashable>)

Adds each object in another given set to the receiving set, if not present.

### Adding and removing entries

func filter(using: NSPredicate)

Evaluates a given predicate against the set’s content and removes from the set those objects for which the predicate returns false.

func remove(Any)

Removes a given object from the set.

func removeAllObjects()

Empties the set of all of its members.

func addObjects(from: [Any])

Adds to the set each object contained in a given array that is not already a member.

