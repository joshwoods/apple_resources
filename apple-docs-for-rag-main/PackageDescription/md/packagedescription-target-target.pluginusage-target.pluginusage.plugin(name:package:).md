

- PackageDescription
- Target
- Target.PluginUsage
-  Target.PluginUsage.plugin(name:package:) 

Case

# Target.PluginUsage.plugin(name:package:)

Specifies the use of a plug-in product in a package dependency.

SwiftPM 5.5+

``` source
case plugin(
    name: String,
    package: String?
)
```

## Parameters 

`name`  

The name of the plug-in target.

`package`  

The name of the package that defines the plug-in target.

## See Also

### Creating a Plugin Usage

static func plugin(name: String) -> Target.PluginUsage

Specifies use of a plugin target in the same package.

