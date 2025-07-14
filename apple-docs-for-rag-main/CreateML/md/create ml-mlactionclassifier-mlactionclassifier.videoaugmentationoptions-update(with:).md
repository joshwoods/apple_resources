

- Create ML
- MLActionClassifier
- MLActionClassifier.VideoAugmentationOptions
-  update(with:) 

Instance Method

# update(with:)

Inserts the given element into the set.

Create MLSwiftmacOS 10.14+

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

### Adding options

func insert(Self.Element) -> (inserted: Bool, memberAfterInsert: Self.Element)

Adds the given element to the option set if it is not already a member.

