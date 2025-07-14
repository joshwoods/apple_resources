

- RealityKit
- ARView
- ARView.DebugOptions
-  subtracting(\_:) 

Instance Method

# subtracting(\_:)

Returns a new set containing the elements of this set that do not occur in the given set.

RealityKitSwiftiOSiPadOSMac CatalystmacOS

``` source
func subtracting(_ other: Self) -> Self
```

## Parameters 

`other`  

A set of the same type as the current set.

## Return Value

A new set.

## Discussion

In the following example, the `nonNeighbors` set is made up of the elements of the `employees` set that are not elements of `neighbors`:

```
let employees: Set = ["Alicia", "Bethany", "Chris", "Diana", "Eric"]
let neighbors: Set = ["Bethany", "Eric", "Forlani", "Greta"]
let nonNeighbors = employees.subtracting(neighbors)
print(nonNeighbors)
// Prints "["Diana", "Chris", "Alicia"]"
```

## See Also

### Adding and removing options

func insert(Self.Element) -> (inserted: Bool, memberAfterInsert: Self.Element)

Adds the given element to the option set if it is not already a member.

func update(with: Self.Element) -> Self.Element?

Inserts the given element into the set.

func remove(Self.Element) -> Self.Element?

Removes the given element and all elements subsumed by it.

func subtract(Self)

Removes the elements of the given set from this set.

