

- PackageDescription
-  PluginCommandIntent 

Enumeration

# PluginCommandIntent

The intended use case of the command plug-in.

SwiftPM 5.6+

``` source
enum PluginCommandIntent
```

## Topics

### Creating a Command Intent

static func documentationGeneration() -> PluginCommandIntent

The plugin generates documentation.

static func sourceCodeFormatting() -> PluginCommandIntent

The plug-in formats source code.

case custom(verb: String, description: String)

A custom command plug-in intent.

### Enumeration Cases

case documentationGeneration

The plug-in generates documentation.

case sourceCodeFormatting

The plug-in formats source code.

## See Also

### Creating a Plugin Target

static func plugin(name: String, capability: Target.PluginCapability, dependencies: [Target.Dependency], path: String?, exclude: [String], sources: [String]?) -> Target

Defines a new package plugin target.

Deprecated

var pluginCapability: Target.PluginCapability?

The capability provided by a package plug-in target.

enum PluginCapability

The different types of capability that a plug-in can provide.

enum PluginPermission

The type of permission a plug-in requires.

