

- Swift Testing
- Comment
-  Comment.RawValue 

Type Alias

# Comment.RawValue

The raw type that can be used to represent all values of the conforming type.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSSwift 6.0+Xcode 16.0+

``` source
typealias RawValue = String
```

## Discussion

Every distinct value of the conforming type has a corresponding unique value of the `RawValue` type, but there may be values of the `RawValue` type that don’t have a corresponding value of the conforming type.

