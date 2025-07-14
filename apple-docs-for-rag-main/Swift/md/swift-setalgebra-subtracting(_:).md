

- Swift
- SetAlgebra
-  subtracting(\_:) 

Instance Method

# subtracting(\_:)

Returns a new set containing the elements of this set that do not occur in the given set.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func subtracting(_ other: Self) -> Self
```

**Required** Default implementation provided.

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

## Default Implementations

### SetAlgebra Implementations

func subtracting(Self) -> Self

Returns a new set containing the elements of this set that do not occur in the given set.

