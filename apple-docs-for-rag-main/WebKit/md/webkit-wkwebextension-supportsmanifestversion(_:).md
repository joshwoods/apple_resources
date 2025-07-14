

- WebKit
- WKWebExtension
-  supportsManifestVersion(\_:) 

Instance Method

# supportsManifestVersion(\_:)

Checks if a manifest version is supported by the extension.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
func supportsManifestVersion(_ manifestVersion: Double) -> Bool
```

## Parameters 

`manifestVersion`  

The version number to check.

## Return Value

Returns `YES` if the extension specified a manifest version that is greater than or equal to `manifestVersion`.

