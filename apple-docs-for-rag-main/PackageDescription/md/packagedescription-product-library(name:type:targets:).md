

- PackageDescription
- Product
-  library(name:type:targets:) 

Type Method

# library(name:type:targets:)

Creates a library product to allow clients that declare a dependency on this package to use the package’s functionality.

``` source
static func library(
    name: String,
    type: Product.Library.LibraryType? = nil,
    targets: [String]
) -> Product
```

## Parameters 

`name`  

The name of the library product.

`type`  

The optional type of the library that’s used to determine how to link to the library. Leave this parameter so Swift Package Manager can choose between static or dynamic linking (recommended). If you don’t support both linkage types, use Product.Library.LibraryType.static or Product.Library.LibraryType.dynamic for this parameter.

`targets`  

The targets that are bundled into a library product.

## Return Value

A `Product` instance.

## Discussion

A library’s product can be either statically or dynamically linked. It’s recommended that you don’t explicitly declare the type of library, so Swift Package Manager can choose between static or dynamic linking based on the preference of the package’s consumer.

## See Also

### Creating a Library Product

class Library

The library product of a Swift package.

