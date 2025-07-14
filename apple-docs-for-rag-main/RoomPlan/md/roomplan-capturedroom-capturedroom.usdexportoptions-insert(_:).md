

- RoomPlan
- CapturedRoom
- CapturedRoom.USDExportOptions
-  insert(\_:) 

Instance Method

# insert(\_:)

Adds the given element to the option set if it is not already a member.

RoomPlanSwiftiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
@discardableResult
mutating func insert(_ newMember: Self.Element) -> (inserted: Bool, memberAfterInsert: Self.Element)
```

Available when `Self` is `Self.Element`.

## Parameters 

`newMember`  

The element to insert.

## Return Value

`(true, newMember)` if `newMember` was not contained in `self`. Otherwise, returns `(false, oldMember)`, where `oldMember` is the member of the set equal to `newMember`.

## Discussion

In the following example, the `.secondDay` shipping option is added to the `freeOptions` option set if `purchasePrice` is greater than 50.0. For the `ShippingOptions` declaration, see the `OptionSet` protocol discussion.

```
let purchasePrice = 87.55

var freeOptions: ShippingOptions = [.standard, .priority]
if purchasePrice > 50 {
    freeOptions.insert(.secondDay)
}
print(freeOptions.contains(.secondDay))
// Prints "true"
```

