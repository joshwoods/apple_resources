

- PackageDescription
- Product
- Product.Library
- Product.Library.LibraryType
-  hash(into:) 

Instance Method

# hash(into:)

Hashes the essential components of this value by feeding them into the given hasher.

PackageDescriptionSwift

``` source
func hash(into hasher: inout Hasher)
```

Available when `Self` conforms to `Hashable` and `RawValue` conforms to `Hashable`.

## Discussion

Implement this method to conform to the Hashable protocol. The components used for hashing must be the same as the components compared in your type’s == operator implementation. Call hasher.combine(\_:) with each of these components.

Important

Never call finalize() on hasher. Doing so may become a compile-time error in the future.

## See Also

### Hashing

var hashValue: Int

The library type’s hash value.

