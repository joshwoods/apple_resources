

- RealityKit
- IKComponent
- IKComponent.ConstraintCollection
-  first 

Instance Property

# first

The first element of the collection.

RealityKitSwiftiOSiPadOSMac CatalystmacOSvisionOS

``` source
var first: Self.Element? { get }
```

## Discussion

If the collection is empty, the value of this property is `nil`.

```
let numbers = [10, 20, 30, 40, 50]
if let firstNumber = numbers.first {
    print(firstNumber)
}
// Prints "10"
```

