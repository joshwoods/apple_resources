

- WebKit
- WKWebExtension
-  manifestVersion 

Instance Property

# manifestVersion

The parsed manifest version, or `0` if there is no version specified in the manifest.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
var manifestVersion: Double { get }
```

## Discussion

Note

A unsupportedManifestVersion error will be reported if the manifest version isn’t specified.

