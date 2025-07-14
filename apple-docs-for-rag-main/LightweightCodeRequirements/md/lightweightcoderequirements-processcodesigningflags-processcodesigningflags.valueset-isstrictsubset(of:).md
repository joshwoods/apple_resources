

- LightweightCodeRequirements
- ProcessCodeSigningFlags
- ProcessCodeSigningFlags.ValueSet
-  isStrictSubset(of:) 

Instance Method

# isStrictSubset(of:)

Returns a Boolean value that indicates whether this set is a strict subset of the given set.

LightweightCodeRequirementsSwiftiOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+tvOSvisionOSwatchOS

``` source
func isStrictSubset(of other: Self) -> Bool
```

## Parameters 

`other`  

A set of the same type as the current set.

## Return Value

`true` if the set is a strict subset of `other`; otherwise, `false`.

## Discussion

Set *A* is a strict subset of another set *B* if every member of *A* is also a member of *B* and *B* contains at least one element that is not a member of *A*.

```
let employees: Set = ["Alicia", "Bethany", "Chris", "Diana", "Eric"]
let attendees: Set = ["Alicia", "Bethany", "Diana"]
print(attendees.isStrictSubset(of: employees))
// Prints "true"

// A set is never a strict subset of itself:
print(attendees.isStrictSubset(of: attendees))
// Prints "false"
```

