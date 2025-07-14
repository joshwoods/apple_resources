

- PackageDescription
-  CXXLanguageStandard 

Enumeration

# CXXLanguageStandard

The supported C++ language standard you use to compile C++ sources in the package.

``` source
enum CXXLanguageStandard
```

## Overview

Aliases are available for some C++ language standards. For example, use `cxx98` or `cxx03` for the “ISO C++ 1998 with amendments” standard. To learn more, see C++ Support in Clang.

## Topics

### Enumeration Cases

case cxx03

The identifier for the ISO C++ 1998 language standard with amendments.

case cxx11

The identifier for the ISO C++ 2011 language standard with amendments.

case cxx14

The identifier for the ISO C++ 2014 language standard with amendments.

case cxx1z

The identifier for the ISO C++ 2017 language standard with amendments.

Deprecated

case cxx98

The identifier for the ISO C++ 1998 language standard with amendments.

case gnucxx03

The identifier for the ISO C++ 1998 language standard with amendments and GNU extensions.

case gnucxx11

The identifier for the ISO C++ 2011 language standard with amendments and GNU extensions.

case gnucxx14

The identifier for the ISO C++ 2014 language standard with amendments and GNU extensions.

case gnucxx1z

The identifier for the ISO C++ 2017 language standard with amendments and GNU extensions.

Deprecated

case gnucxx98

The identifier for the ISO C++ 1998 language standard with amendments and GNU extensions.

case cxx17

The identifier for the ISO C++ 2017 language standard with amendments.

case cxx20

The identifier for the ISO C++ 2020 language standard.

case cxx2b

The identifier for the ISO C++ 2023 draft language standard.

case gnucxx17

The identifier for the ISO C++ 2017 language standard with amendments and GNU extensions.

case gnucxx20

The identifier for the ISO C++ 2020 language standard with GNU extensions.

case gnucxx2b

The identifier for the ISO C++ 2023 draft language standard with GNU extensions.

### Hashing

func hash(into: inout Hasher)

Hashes the C++ language standard by feeding the item into the given hasher.

var hashValue: Int

The hash value for the C++ language standard.

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

enum CLanguageStandard

The supported C language standard you use to compile C sources in the package.

var swiftLanguageVersions: [SwiftVersion]?

Legacy property name, accesses value of `swiftLanguageModes`

Deprecated

var cLanguageStandard: CLanguageStandard?

The C language standard to use for all C targets in this package.

var cxxLanguageStandard: CXXLanguageStandard?

The C++ language standard to use for all C++ targets in this package.

