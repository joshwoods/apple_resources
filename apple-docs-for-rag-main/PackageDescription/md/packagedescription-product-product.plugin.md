

- PackageDescription
- Product
-  Product.Plugin 

Class

# Product.Plugin

The plug-in product of a Swift package.

``` source
final class Plugin
```

## Topics

### Describing a plug-in product

let targets: [String]

The name of the plug-in target to vend as a product.

## Relationships

### Inherits From

- Product

### Conforms To

- Sendable

## See Also

### Creating a Plugin Product

static func plugin(name: String, targets: [String]) -> Product

Defines a product that vends a package plugin target for use by clients of the package.

