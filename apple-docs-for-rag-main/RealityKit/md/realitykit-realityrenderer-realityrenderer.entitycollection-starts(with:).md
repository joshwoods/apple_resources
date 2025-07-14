

- RealityKit
- RealityRenderer
- RealityRenderer.EntityCollection
-  starts(with:) 

Instance Method

# starts(with:)

Returns a Boolean value indicating whether the initial elements of the sequence are the same as the elements in another sequence.

RealityKitSwiftiOSiPadOSMac CatalystmacOSvisionOS

``` source
func starts(with possiblePrefix: PossiblePrefix) -> Bool where PossiblePrefix : Sequence, Self.Element == PossiblePrefix.Element
```

Available when `Element` conforms to `Equatable`.

## Parameters 

`possiblePrefix`  

A sequence to compare to this sequence.

## Return Value

`true` if the initial elements of the sequence are the same as the elements of `possiblePrefix`; otherwise, `false`. If `possiblePrefix` has no elements, the return value is `true`.

## Discussion

This example tests whether one countable range begins with the elements of another countable range.

```
let a = 1...3
let b = 1...10

print(b.starts(with: a))
// Prints "true"
```

Passing a sequence with no elements or an empty collection as `possiblePrefix` always results in `true`.

```
print(b.starts(with: []))
// Prints "true"
```

Complexity

O(*m*), where *m* is the lesser of the length of the sequence and the length of `possiblePrefix`.

