

- PackageDescription
- Target
- Target.PluginCapability
-  buildTool() 

Type Method

# buildTool()

The plug-in is a build tool.

SwiftPM 5.5+

``` source
static func buildTool() -> Target.PluginCapability
```

## Return Value

A plug-in capability that defines a build tool.

## Discussion

The plug-in to apply to each target that uses it, and creates commands that run before or during the build of the target.

## See Also

### Creating a Plugin Capability

case command(intent: PluginCommandIntent, permissions: [PluginPermission])

Specifies that the plug-in provides a user command capability.

