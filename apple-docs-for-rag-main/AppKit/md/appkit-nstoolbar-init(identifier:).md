

- AppKit
- NSToolbar
-  init(identifier:) 

Initializer

# init(identifier:)

Creates a newly allocated toolbar with the specified identifier.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS

``` source
@MainActor
init(identifier: NSToolbar.Identifier)
```

## Parameters 

`identifier`  

A string used by the class to identify the kind of the toolbar.

## Return Value

The initialized toolbar object.

## Discussion

`identifier` is never seen by users and should not be localized. See the identifier property for important information.

## See Also

### Related Documentation

var identifier: NSToolbar.Identifier

The value you use to identify the toolbar in your app.

Toolbar Programming Topics for Cocoa

### Creating an toolbar object

convenience init()

Creates a new toolbar with an empty identifier string.

