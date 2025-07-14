

- PackageDescription
- Product
- Product.Library
- Product.Library.LibraryType
-  Product.Library.LibraryType.RawValue 

Type Alias

# Product.Library.LibraryType.RawValue

The raw type that can be used to represent all values of the conforming type.

``` source
typealias RawValue = String
```

## Discussion

Every distinct value of the conforming type has a corresponding unique value of the `RawValue` type, but there may be values of the `RawValue` type that don’t have a corresponding value of the conforming type.

## See Also

### Accessing the Raw Value

var rawValue: String

The corresponding value of the raw type.

