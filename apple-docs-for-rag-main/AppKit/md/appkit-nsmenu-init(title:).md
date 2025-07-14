

- AppKit
- NSMenu
-  init(title:) 

Initializer

# init(title:)

Initializes and returns a menu having the specified title and with autoenabling of menu items turned on.

macOS

``` source
init(title: String)
```

## Parameters 

`title`  

The title to assign to the menu.

## Return Value

The initialized `NSMenu` object or `nil` if the object could not be initialized.

## Discussion

This method is the designated initializer for the class.

## See Also

### Related Documentation

var autoenablesItems: Bool

Indicates whether the menu automatically enables and disables its menu items.

### Creating an NSMenu Object

init(coder: NSCoder)

