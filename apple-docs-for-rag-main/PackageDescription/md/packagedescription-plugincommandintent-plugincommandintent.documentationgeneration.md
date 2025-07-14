

- PackageDescription
- PluginCommandIntent
-  PluginCommandIntent.documentationGeneration 

Case

# PluginCommandIntent.documentationGeneration

The plug-in generates documentation.

SwiftPM 5.6+

``` source
case documentationGeneration
```

## Discussion

The command used to generate documentation, either by parsing the package contents directly or by using the build system support for generating symbol graphs. Invoked by a `generate-documentation` verb to `swift package`.

