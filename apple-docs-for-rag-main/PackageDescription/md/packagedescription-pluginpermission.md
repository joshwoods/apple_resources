

- PackageDescription
-  PluginPermission 

Enumeration

# PluginPermission

The type of permission a plug-in requires.

SwiftPM 5.6+

``` source
enum PluginPermission
```

## Overview

Supported types are PluginPermission.allowNetworkConnections(scope:reason:) and PluginPermission.writeToPackageDirectory(reason:).

## Topics

### Create a permission

case allowNetworkConnections(scope: PluginNetworkPermissionScope, reason: String)

Create a permission to make network connections.

case writeToPackageDirectory(reason: String)

Create a permission to modify files in the package’s directory.

### Allow network connection

enum PluginNetworkPermissionScope

The scope of a network permission.

## See Also

### Creating a Plugin Target

static func plugin(name: String, capability: Target.PluginCapability, dependencies: [Target.Dependency], path: String?, exclude: [String], sources: [String]?) -> Target

Defines a new package plugin target.

Deprecated

var pluginCapability: Target.PluginCapability?

The capability provided by a package plug-in target.

enum PluginCapability

The different types of capability that a plug-in can provide.

enum PluginCommandIntent

The intended use case of the command plug-in.

