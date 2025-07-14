

- PackageDescription
- Target
-  Target.PluginCapability 

Enumeration

# Target.PluginCapability

The different types of capability that a plug-in can provide.

``` source
enum PluginCapability
```

## Overview

In this version of SwiftPM, only build tool and command plug-ins are supported; this enumeration will be extended as new plug-in capabilities are added.

## Topics

### Creating a Plugin Capability

static func buildTool() -> Target.PluginCapability

The plug-in is a build tool.

case command(intent: PluginCommandIntent, permissions: [PluginPermission])

Specifies that the plug-in provides a user command capability.

### Enumeration Cases

case buildTool

Specifies that the plug-in provides a build tool capability.

## See Also

### Creating a Plugin Target

static func plugin(name: String, capability: Target.PluginCapability, dependencies: [Target.Dependency], path: String?, exclude: [String], sources: [String]?) -> Target

Defines a new package plugin target.

Deprecated

var pluginCapability: Target.PluginCapability?

The capability provided by a package plug-in target.

enum PluginCommandIntent

The intended use case of the command plug-in.

enum PluginPermission

The type of permission a plug-in requires.

