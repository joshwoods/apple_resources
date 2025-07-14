

- FSKit
- FSItem
- FSItem.Attribute
-  remove(\_:) 

Instance Method

# remove(\_:)

Removes the given element and all elements subsumed by it.

FSKitSwiftmacOS 15.4+

``` source
@discardableResult
mutating func remove(_ member: Self.Element) -> Self.Element?
```

Available when `Self` is `Self.Element`.

## Parameters 

`member`  

The element of the set to remove.

## Return Value

The intersection of `[member]` and the set, if the intersection was nonempty; otherwise, `nil`.

## Discussion

In the following example, the `.priority` shipping option is removed from the `options` option set. Attempting to remove the same shipping option a second time results in `nil`, because `options` no longer contains `.priority` as a member.

```
var options: ShippingOptions = [.secondDay, .priority]
let priorityOption = options.remove(.priority)
print(priorityOption == .priority)
// Prints "true"

print(options.remove(.priority))
// Prints "nil"
```

In the next example, the `.express` element is passed to `remove(_:)`. Although `.express` is not a member of `options`, `.express` subsumes the remaining `.secondDay` element of the option set. Therefore, `options` is emptied and the intersection between `.express` and `options` is returned.

```
let expressOption = options.remove(.express)
print(expressOption == .express)
// Prints "false"
print(expressOption == .secondDay)
// Prints "true"
```

