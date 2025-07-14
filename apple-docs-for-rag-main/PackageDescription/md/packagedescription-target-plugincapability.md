

- PackageDescription
- Target
-  pluginCapability 

Instance Property

# pluginCapability

The capability provided by a package plug-in target.

SwiftPM 5.5+

``` source
final var pluginCapability: Target.PluginCapability?
```

## See Also

### Creating a Plugin Target

static func plugin(name: String, capability: Target.PluginCapability, dependencies: [Target.Dependency], path: String?, exclude: [String], sources: [String]?) -> Target

Defines a new package plugin target.

Deprecated

enum PluginCapability

The different types of capability that a plug-in can provide.

enum PluginCommandIntent

The intended use case of the command plug-in.

enum PluginPermission

The type of permission a plug-in requires.

