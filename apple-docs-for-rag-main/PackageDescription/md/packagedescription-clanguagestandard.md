

- PackageDescription
-  CLanguageStandard 

Enumeration

# CLanguageStandard

The supported C language standard you use to compile C sources in the package.

``` source
enum CLanguageStandard
```

## Topics

### Enumeration Cases

case c11

The identifier for the ISO C 2011 language standard.

case c17

The identifier for the ISO C 2017 language stadard.

case c18

The identifier for the ISO C 2017 language standard.

case c2x

The identifier for the ISO C2x draft language standard.

case c89

The identifier for the ISO C 1990 language standard.

case c90

The identifier for the ISO C 1990 language standard.

case c99

The identifier for the ISO C 1999 language standard.

case gnu11

The identifier for the ISO C 2011 language standard with GNU extensions.

case gnu17

The identifier for the ISO C 2017 language standard with GNU extensions.

case gnu18

The identifier for the ISO C 2017 language standard with GNU extensions.

case gnu2x

The identifier for the ISO C2x draft language standard with GNU extensions.

case gnu89

The identifier for the ISO C 1990 language standard with GNU extensions.

case gnu90

The identifier for the ISO C 1990 language standard with GNU extensions.

case gnu99

The identifier for the ISO C 1999 language standard with GNU extensions.

case iso9899_1990

The identifier for the ISO C 1990 language standard.

case iso9899_199409

The identifier for the ISO C 1990 language standard with amendment 1.

case iso9899_1999

The identifier for the ISO C 1999 language standard.

case iso9899_2011

The identifier for the ISO C 2011 language standard.

case iso9899_2017

The identifier for the ISO C 2017 language standard.

case iso9899_2018

The identifier for the ISO C 2017 language standard.

### Hashing

func hash(into: inout Hasher)

Hashes the C language standard by feeding the item into the given hasher.

var hashValue: Int

The hash value for the C language standard.

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

### Declaring Supported Languages

typealias SwiftVersion

Type alias to previous name for backward source compatibility

Deprecated

enum CXXLanguageStandard

The supported C++ language standard you use to compile C++ sources in the package.

var swiftLanguageVersions: [SwiftVersion]?

Legacy property name, accesses value of `swiftLanguageModes`

Deprecated

var cLanguageStandard: CLanguageStandard?

The C language standard to use for all C targets in this package.

var cxxLanguageStandard: CXXLanguageStandard?

The C++ language standard to use for all C++ targets in this package.

