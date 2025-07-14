

- AppKit
- NSToolbar
-  configuration Deprecated

Instance Property

# configuration

A dictionary containing the current configuration details for the toolbar.

macOS 10.0–15.0Deprecated

``` source
@MainActor
var configuration: [String : Any] { get }
```

Deprecated

Use -itemIdentifiers and -displayMode instead.

## Discussion

Use this property to retrieve the toolbar’s configuration details so you can save them to disk yourself. The dictionary in this property contains the identifiers of the current toolbar items and the values of important properties such as displayMode and isVisible.

## See Also

### Autosaving the configuration

var autosavesConfiguration: Bool

A Boolean value that indicates whether the toolbar autosaves its configuration.

func setConfiguration([String : Any])

Specifies the new configuration details for the toolbar.

Deprecated

