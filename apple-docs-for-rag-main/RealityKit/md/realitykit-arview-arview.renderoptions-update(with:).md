

- RealityKit
- ARView
- ARView.RenderOptions
-  update(with:) 

Instance Method

# update(with:)

Inserts the given element into the set.

RealityKitSwiftiOSiPadOSMac Catalyst

``` source
@discardableResult
mutating func update(with newMember: Self.Element) -> Self.Element?
```

Available when `Self` is `Self.Element`.

## Return Value

The intersection of `[newMember]` and the set if the intersection was nonempty; otherwise, `nil`.

## Discussion

If `newMember` is not contained in the set but subsumes current members of the set, the subsumed members are returned.

```
var options: ShippingOptions = [.secondDay, .priority]
let replaced = options.update(with: .express)
print(replaced == .secondDay)
// Prints "true"
```

## See Also

### Adding and removing options

func insert(Self.Element) -> (inserted: Bool, memberAfterInsert: Self.Element)

Adds the given element to the option set if it is not already a member.

func remove(Self.Element) -> Self.Element?

Removes the given element and all elements subsumed by it.

func subtract(Self)

Removes the elements of the given set from this set.

func subtracting(Self) -> Self

Returns a new set containing the elements of this set that do not occur in the given set.

