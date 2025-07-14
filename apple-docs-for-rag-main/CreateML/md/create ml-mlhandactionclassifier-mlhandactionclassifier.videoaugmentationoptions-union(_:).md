

- Create ML
- MLHandActionClassifier
- MLHandActionClassifier.VideoAugmentationOptions
-  union(\_:) 

Instance Method

# union(\_:)

Returns a new option set of the elements contained in this set, in the given set, or in both.

Create MLSwiftiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+visionOS 1.0+

``` source
func union(_ other: Self) -> Self
```

## Parameters 

`other`  

An option set.

## Return Value

A new option set made up of the elements contained in this set, in `other`, or in both.

## Discussion

This example uses the `union(_:)` method to add two more shipping options to the default set.

```
let defaultShipping = ShippingOptions.standard
let memberShipping = defaultShipping.union([.secondDay, .priority])
print(memberShipping.contains(.priority))
// Prints "true"
```

