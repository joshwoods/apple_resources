

- RealityKit
- ARView
- ARView.RenderOptions
-  insert(\_:) 

Instance Method

# insert(\_:)

Adds the given element to the option set if it is not already a member.

RealityKitSwiftiOSiPadOSMac Catalyst

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

## See Also

### Adding and removing options

func update(with: Self.Element) -> Self.Element?

Inserts the given element into the set.

func remove(Self.Element) -> Self.Element?

Removes the given element and all elements subsumed by it.

func subtract(Self)

Removes the elements of the given set from this set.

func subtracting(Self) -> Self

Returns a new set containing the elements of this set that do not occur in the given set.

