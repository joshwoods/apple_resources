

- AppKit
- NSToolbar
-  setConfiguration(\_:) Deprecated

Instance Method

# setConfiguration(\_:)

Specifies the new configuration details for the toolbar.

macOS 10.0–15.0Deprecated

``` source
@MainActor
func setConfiguration(_ configDict: [String : Any])
```

Deprecated

Use -setItemIdentifiers: and -setDisplayMode: instead.

## Parameters 

`configDict`  

A dictionary with the toolbar configuration details. The toolbar ignores any keys it doesn’t recognize. Typically, you save the original configuration dictionary from the configuration property to disk and recreate it before passing it in this parameter.

## Discussion

If you implement your own autosave mechanism, call this method to restore the configuration of your toolbar to a previously saved state. The dictionary you read from disk must match the format of the dictionary in the configuration property.

## See Also

### Autosaving the configuration

var autosavesConfiguration: Bool

A Boolean value that indicates whether the toolbar autosaves its configuration.

var configuration: [String : Any]

A dictionary containing the current configuration details for the toolbar.

Deprecated

