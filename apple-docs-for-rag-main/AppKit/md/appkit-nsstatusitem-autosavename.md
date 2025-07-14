

- AppKit
- NSStatusItem
-  autosaveName 

Instance Property

# autosaveName

A unique name for saving and restoring information about a status item.

macOS 10.12+

``` source
var autosaveName: NSStatusItem.AutosaveName! { get set }
```

## Discussion

If you do not provide an autosave name for a status item, the system automatically chooses a unique name. Setting this property to Nil resets it to the automatically chosen name.

Applications with multiple status items should set an autosave name after creating each item.

## See Also

### Setting the Autosave Name

typealias AutosaveName

