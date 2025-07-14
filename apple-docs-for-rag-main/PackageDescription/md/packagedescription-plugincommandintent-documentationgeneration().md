

- PackageDescription
- PluginCommandIntent
-  documentationGeneration() 

Type Method

# documentationGeneration()

The plugin generates documentation.

SwiftPM 5.6+

``` source
static func documentationGeneration() -> PluginCommandIntent
```

## Return Value

A `PluginCommandIntent` instance.

## Discussion

The intent of the command is to generate documentation, either by parsing the package contents directly or by using the build system support for generating symbol graphs. Invoked by a `generate-documentation` verb to `swift package`.

## See Also

### Creating a Command Intent

static func sourceCodeFormatting() -> PluginCommandIntent

The plug-in formats source code.

case custom(verb: String, description: String)

A custom command plug-in intent.

