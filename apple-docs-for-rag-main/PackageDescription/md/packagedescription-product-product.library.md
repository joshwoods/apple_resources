

- PackageDescription
- Product
-  Product.Library 

Class

# Product.Library

The library product of a Swift package.

``` source
final class Library
```

## Topics

### Describing a Library Product

let targets: [String]

The names of the targets in this product.

let type: Product.Library.LibraryType?

The type of the library.

enum LibraryType

The different types of a library product.

## Relationships

### Inherits From

- Product

### Conforms To

- Sendable

## See Also

### Creating a Library Product

static func library(name: String, type: Product.Library.LibraryType?, targets: [String]) -> Product

Creates a library product to allow clients that declare a dependency on this package to use the package’s functionality.

