

- PackageDescription
- PluginCommandIntent
-  PluginCommandIntent.custom(verb:description:) 

Case

# PluginCommandIntent.custom(verb:description:)

A custom command plug-in intent.

SwiftPM 5.6+

``` source
case custom(
    verb: String,
    description: String
)
```

## Parameters 

`verb`  

The invocation verb of the plug-in.

`description`  

A human readable description of the plug-in’s role.

## Discussion

Use this case when none of the predefined cases fulfill the role of the plug-in.

## See Also

### Creating a Command Intent

static func documentationGeneration() -> PluginCommandIntent

The plugin generates documentation.

static func sourceCodeFormatting() -> PluginCommandIntent

The plug-in formats source code.

