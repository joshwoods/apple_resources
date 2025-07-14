

- AppKit
- NSUserInterfaceItemIdentification
-  identifier 

Instance Property

# identifier

A string that identifies the user interface item.

macOS

``` source
var identifier: NSUserInterfaceItemIdentifier? { get set }
```

**Required**

## Discussion

Identifiers are used during window restoration operations to uniquely identify the windows of the application. You can set the value of this string programmatically or in Interface Builder. If you create an item in Interface Builder and do not set a value for this string, a unique value is created for the item when the nib file is loaded. For programmatically created views, you typically set this value after creating the item but before adding it to a window.

You should not change the value of a window’s identifier after adding any views to the window. For views and controls in a window, the value you specify for this string must be unique on a per-window basis.

The slash (`/`), backslash (`\`), or colon (`:`) characters are reserved and must not be used in your custom identifiers. Similarly, Apple reserves all identifiers beginning with an underscore (`_`) character. Applications and frameworks should use a consistent prefix for their identifiers to avoid collisions with other frameworks. For a list of prefixes used by the system frameworks, see OS X Frameworks in Mac Technology Overview.

If you are subclassing a class from one of the system frameworks, do not override the accessor methods of this protocol.

## See Also

### Accessing the User Interface Identifier

struct NSUserInterfaceItemIdentifier

