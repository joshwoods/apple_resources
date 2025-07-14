

- PackageDescription
- Package
-  cLanguageStandard 

Instance Property

# cLanguageStandard

The C language standard to use for all C targets in this package.

``` source
final var cLanguageStandard: CLanguageStandard?
```

## See Also

### Declaring Supported Languages

typealias SwiftVersion

Type alias to previous name for backward source compatibility

Deprecated

enum CLanguageStandard

The supported C language standard you use to compile C sources in the package.

enum CXXLanguageStandard

The supported C++ language standard you use to compile C++ sources in the package.

var swiftLanguageVersions: [SwiftVersion]?

Legacy property name, accesses value of `swiftLanguageModes`

Deprecated

var cxxLanguageStandard: CXXLanguageStandard?

The C++ language standard to use for all C++ targets in this package.

