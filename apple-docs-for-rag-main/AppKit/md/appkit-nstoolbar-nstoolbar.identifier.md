

- AppKit
- NSToolbar
-  NSToolbar.Identifier 

Type Alias

# NSToolbar.Identifier

A string value that you use to differentiate your app’s toolbars.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS

``` source
typealias Identifier = String
```

## Discussion

Multiple toolbar objects can have the same identifier. If two or more toolbars share an identifier, the system synchronizes the state of the toolbars and displays the same items for each one.

## See Also

### Getting the toolbar’s identity

var identifier: NSToolbar.Identifier

The value you use to identify the toolbar in your app.

