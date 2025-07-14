

- RealityKit
- AnimationLibraryComponent
- AnimationLibraryComponent.AnimationCollection
- AnimationLibraryComponent.AnimationCollection.Index
-  ...(\_:\_:) 

Operator

# ...(\_:\_:)

Returns a closed range that contains both of its bounds.

RealityKitSwiftiOSiPadOSMac CatalystmacOSvisionOS

``` source
static func ... (minimum: Self, maximum: Self) -> ClosedRange
```

## Parameters 

`minimum`  

The lower bound for the range.

`maximum`  

The upper bound for the range.

## Discussion

Use the closed range operator (`...`) to create a closed range of any type that conforms to the `Comparable` protocol. This example creates a `ClosedRange` from “a” up to, and including, “z”.

```
let lowercase = "a"..."z"
print(lowercase.contains("z"))
// Prints "true"
```

Precondition

`minimum 

