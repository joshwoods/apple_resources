

- PackageDescription
- PluginCommandIntent
-  sourceCodeFormatting() 

Type Method

# sourceCodeFormatting()

The plug-in formats source code.

SwiftPM 5.6+

``` source
static func sourceCodeFormatting() -> PluginCommandIntent
```

## Return Value

A `PluginCommandIntent` instance.

## Discussion

The intent of the command is to modify the source code in the package based on a set of rules. Invoked by a `format-source-code` verb to `swift package`.

## See Also

### Creating a Command Intent

static func documentationGeneration() -> PluginCommandIntent

The plugin generates documentation.

case custom(verb: String, description: String)

A custom command plug-in intent.

