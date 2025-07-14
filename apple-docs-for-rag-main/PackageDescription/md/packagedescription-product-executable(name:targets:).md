

- PackageDescription
- Product
-  executable(name:targets:) 

Type Method

# executable(name:targets:)

Creates an executable package product.

``` source
static func executable(
    name: String,
    targets: [String]
) -> Product
```

## Parameters 

`name`  

The name of the executable product.

`targets`  

The targets to bundle into an executable product.

## Return Value

A `Product` instance.

## See Also

### Creating an Executable Product

class Executable

The executable product of a Swift package.

