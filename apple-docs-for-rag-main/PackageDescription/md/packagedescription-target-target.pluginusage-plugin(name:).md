

- PackageDescription
- Target
- Target.PluginUsage
-  plugin(name:) 

Type Method

# plugin(name:)

Specifies use of a plugin target in the same package.

SwiftPM 5.5+

``` source
static func plugin(name: String) -> Target.PluginUsage
```

## Parameters 

`name`  

The name of the plugin target.

## Return Value

A `PluginUsage` instance.

## See Also

### Creating a Plugin Usage

case plugin(name: String, package: String?)

Specifies the use of a plug-in product in a package dependency.

