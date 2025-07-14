

- PackageDescription
- Product
- Product.Library
-  Product.Library.LibraryType 

Enumeration

# Product.Library.LibraryType

The different types of a library product.

``` source
enum LibraryType
```

## Topics

### Enumeration Cases

case dynamic

A dynamically linked library.

case `static`

A statically linked library.

### Hashing

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

var hashValue: Int

The library type’s hash value.

### Operator Functions

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Creating a Value

init?(rawValue: String)

Creates a new instance with the specified raw value.

### Accessing the Raw Value

var rawValue: String

The corresponding value of the raw type.

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- RawRepresentable

## See Also

### Describing a Library Product

let targets: [String]

The names of the targets in this product.

let type: Product.Library.LibraryType?

The type of the library.

