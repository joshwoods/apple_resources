

- App Intents
- ConfirmationConditions
-  subtract(\_:) 

Instance Method

# subtract(\_:)

Removes the elements of the given set from this set.

App IntentsSwiftiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
mutating func subtract(_ other: Self)
```

## Parameters 

`other`  

A set of the same type as the current set.

## Discussion

In the following example, the elements of the `employees` set that are also members of the `neighbors` set are removed. In particular, the names `"Bethany"` and `"Eric"` are removed from `employees`.

```
var employees: Set = ["Alicia", "Bethany", "Chris", "Diana", "Eric"]
let neighbors: Set = ["Bethany", "Eric", "Forlani", "Greta"]
employees.subtract(neighbors)
print(employees)
// Prints "["Diana", "Chris", "Alicia"]"
```

