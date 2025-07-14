

- PackageDescription
- Product
-  Product.Executable 

Class

# Product.Executable

The executable product of a Swift package.

``` source
final class Executable
```

## Topics

### Describing an executable product

let targets: [String]

The names of the targets in this product.

## Relationships

### Inherits From

- Product

### Conforms To

- Sendable

## See Also

### Creating an Executable Product

static func executable(name: String, targets: [String]) -> Product

Creates an executable package product.

