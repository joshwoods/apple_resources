

- FamilyControls
- FamilyControlsError
-  FamilyControlsError.RawValue 

Type Alias

# FamilyControlsError.RawValue

The raw type that can be used to represent all values of the conforming type.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+

``` source
typealias RawValue = Int
```

## Discussion

Every distinct value of the conforming type has a corresponding unique value of the `RawValue` type, but there may be values of the `RawValue` type that don’t have a corresponding value of the conforming type.

