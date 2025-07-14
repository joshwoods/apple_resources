

- XCUIAutomation
- XCUIAccessibilityAuditType
-  isSubset(of:) 

Instance Method

# isSubset(of:)

Returns a Boolean value that indicates whether the set is a subset of another set.

XCUIAutomationSwiftiOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSXcode 16.3+

``` source
func isSubset(of other: Self) -> Bool
```

## Parameters 

`other`  

A set of the same type as the current set.

## Return Value

`true` if the set is a subset of `other`; otherwise, `false`.

## Discussion

Set *A* is a subset of another set *B* if every member of *A* is also a member of *B*.

```
let employees: Set = ["Alicia", "Bethany", "Chris", "Diana", "Eric"]
let attendees: Set = ["Alicia", "Bethany", "Diana"]
print(attendees.isSubset(of: employees))
// Prints "true"
```

