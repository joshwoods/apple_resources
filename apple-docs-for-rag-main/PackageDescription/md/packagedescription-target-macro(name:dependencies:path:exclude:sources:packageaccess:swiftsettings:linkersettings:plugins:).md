

- PackageDescription
- Target
-  macro(name:dependencies:path:exclude:sources:packageAccess:swiftSettings:linkerSettings:plugins:) 

Type Method

# macro(name:dependencies:path:exclude:sources:packageAccess:swiftSettings:linkerSettings:plugins:)

SwiftPM 5.9+

``` source
static func macro(
    name: String,
    dependencies: [Target.Dependency] = [],
    path: String? = nil,
    exclude: [String] = [],
    sources: [String]? = nil,
    packageAccess: Bool = true,
    swiftSettings: [SwiftSetting]? = nil,
    linkerSettings: [LinkerSetting]? = nil,
    plugins: [Target.PluginUsage]? = nil
) -> Target
```

