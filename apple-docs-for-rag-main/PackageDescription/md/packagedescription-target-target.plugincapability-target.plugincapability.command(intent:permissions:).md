

- PackageDescription
- Target
- Target.PluginCapability
-  Target.PluginCapability.command(intent:permissions:) 

Case

# Target.PluginCapability.command(intent:permissions:)

Specifies that the plug-in provides a user command capability.

SwiftPM 5.6+

``` source
case command(
    intent: PluginCommandIntent,
    permissions: [PluginPermission] = []
)
```

## Parameters 

`intent`  

The semantic intent of the plug-in; either one of the predefined intents, or a custom intent.

`permissions`  

Any permissions needed by the command plug-in. This affects what the sandbox in which the plug-in is run allows. Some permissions may require user approval.

## Discussion

Plug-ins that specify a `command` capability define commands that can run using the SwiftPM command line interface, or in an IDE that supports Swift packages. You can invoke the command manually on one or more targets in a package.

```
swift package 
```

The package can specify the *verb* used to invoke the command.

## See Also

### Creating a Plugin Capability

static func buildTool() -> Target.PluginCapability

The plug-in is a build tool.

