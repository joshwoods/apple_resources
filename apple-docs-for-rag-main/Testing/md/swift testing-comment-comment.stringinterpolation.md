

- Swift Testing
- Comment
-  Comment.StringInterpolation 

Type Alias

# Comment.StringInterpolation

The type each segment of a string literal containing interpolations should be appended to.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSSwift 6.0+Xcode 16.0+

``` source
typealias StringInterpolation = DefaultStringInterpolation
```

## Discussion

The `StringLiteralType` of an interpolation type must match the `StringLiteralType` of the conforming type.

