

- Foundation
- NSMutableSet
-  union(\_:) 

Instance Method

# union(\_:)

Adds each object in another given set to the receiving set, if not present.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func union(_ otherSet: Set)
```

## Parameters 

`otherSet`  

The set of objects to add to the receiving set.

## See Also

### Related Documentation

func add(Any)

Adds a given object to the set, if it is not already a member.

func addObjects(from: [Any])

Adds to the set each object contained in a given array that is not already a member.

### Combining and recombining sets

func minus(Set&lt;AnyHashable>)

Removes each object in another given set from the receiving set, if present.

func intersect(Set&lt;AnyHashable>)

Removes from the receiving set each object that isn’t a member of another given set.

func setSet(Set&lt;AnyHashable>)

Empties the receiving set, then adds each object contained in another given set.

