

- AppKit
- NSToolbar
-  autosavesConfiguration 

Instance Property

# autosavesConfiguration

A Boolean value that indicates whether the toolbar autosaves its configuration.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS

``` source
@MainActor
var autosavesConfiguration: Bool { get set }
```

## Discussion

When the value of this property is true, the toolbar automatically writes any configuration changes to user defaults. It associates the configuration details with the value in its identifier property. If mutliple toolbars share the same identifier, they all share the same configuration settings. When the value of this property is false, the toolbar doesn’t save changes and reverts to the default configuration when the app relaunches.

The default of this property is false.

Important

If you allow people to customize your app’s toolbars, enable this property to save the changes they make. Alternatively, use the configuration property and setConfiguration(_:) method to manage the autosave process yourself.

## See Also

### Related Documentation

var allowsUserCustomization: Bool

A Boolean value that indicates whether users can modify the contents of the toolbar.

### Autosaving the configuration

var configuration: [String : Any]

A dictionary containing the current configuration details for the toolbar.

Deprecated

func setConfiguration([String : Any])

Specifies the new configuration details for the toolbar.

Deprecated

