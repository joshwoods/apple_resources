

- LightweightCodeRequirements
- OnDiskCodeSigningFlags
- OnDiskCodeSigningFlags.ValueSet
-  union(\_:) 

Instance Method

# union(\_:)

Returns a new option set of the elements contained in this set, in the given set, or in both.

LightweightCodeRequirementsSwiftiOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+tvOSvisionOSwatchOS

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

