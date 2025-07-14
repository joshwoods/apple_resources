

- Create ML
- MLActionClassifier
- MLActionClassifier.VideoAugmentationOptions
-  contains(\_:) 

Instance Method

# contains(\_:)

Returns a Boolean value that indicates whether a given element is a member of the option set.

Create MLSwiftmacOS 10.14+

``` source
func contains(_ member: Self) -> Bool
```

Available when `Self` is `Self.Element`.

## Parameters 

`member`  

The element to look for in the option set.

## Return Value

`true` if the option set contains `member`; otherwise, `false`.

## Discussion

This example uses the `contains(_:)` method to check whether next-day shipping is in the `availableOptions` instance.

```
let availableOptions = ShippingOptions.express
if availableOptions.contains(.nextDay) {
    print("Next day shipping available")
}
// Prints "Next day shipping available"
```

## See Also

### Inspecting options

var isEmpty: Bool

A Boolean value that indicates whether the set has no elements.

let rawValue: Int

The corresponding value of the raw type.

