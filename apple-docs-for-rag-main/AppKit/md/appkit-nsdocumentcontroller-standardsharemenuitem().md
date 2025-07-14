

- AppKit
- NSDocumentController
-  standardShareMenuItem() 

Instance Method

# standardShareMenuItem()

Returns a menu item that your app uses for sharing the current document.

macOS 10.13+

``` source
@MainActor
func standardShareMenuItem() -> NSMenuItem
```

## Return Value

An NSMenuItem for the Share menu.

## Discussion

Use this method to perform custom placement of the Share menu if your NSDocument subclass returns `false` for allowsAutomaticShareMenu.

## See Also

### Sharing

var allowsAutomaticShareMenu: Bool

A Boolean value that the system uses to insert a Share menu in the File menu.

