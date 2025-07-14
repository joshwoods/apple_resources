

- PackageDescription
-  SwiftVersion Deprecated

Type Alias

# SwiftVersion

Type alias to previous name for backward source compatibility

SwiftPMDeprecated

``` source
typealias SwiftVersion = SwiftLanguageMode
```

## See Also

### Declaring Supported Languages

enum CLanguageStandard

The supported C language standard you use to compile C sources in the package.

enum CXXLanguageStandard

The supported C++ language standard you use to compile C++ sources in the package.

var swiftLanguageVersions: [SwiftVersion]?

Legacy property name, accesses value of `swiftLanguageModes`

Deprecated

var cLanguageStandard: CLanguageStandard?

The C language standard to use for all C targets in this package.

var cxxLanguageStandard: CXXLanguageStandard?

The C++ language standard to use for all C++ targets in this package.

