

- Core HID
- HIDUsage
- HIDUsage.BarcodeScannerUsage
-  HIDUsage.BarcodeScannerUsage.RawValue 

Type Alias

# HIDUsage.BarcodeScannerUsage.RawValue

The raw type that can be used to represent all values of the conforming type.

macOS 15.0+

``` source
typealias RawValue = UInt16
```

## Discussion

Every distinct value of the conforming type has a corresponding unique value of the `RawValue` type, but there may be values of the `RawValue` type that don’t have a corresponding value of the conforming type.

