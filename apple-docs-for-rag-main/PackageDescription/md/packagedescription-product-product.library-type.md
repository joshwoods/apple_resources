

- PackageDescription
- Product
- Product.Library
-  type 

Instance Property

# type

The type of the library.

``` source
final let type: Product.Library.LibraryType?
```

## Discussion

If the type is unspecified, the Swift Package Manager automatically chooses a type based on the client’s preference.

## See Also

### Describing a Library Product

let targets: [String]

The names of the targets in this product.

enum LibraryType

The different types of a library product.

