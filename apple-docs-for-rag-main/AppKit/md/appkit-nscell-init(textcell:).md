

- AppKit
- NSCell
-  init(textCell:) 

Initializer

# init(textCell:)

Returns an NSCell object initialized with the specified string and set to have the cell’s default menu.

macOS

``` source
@MainActor
init(textCell string: String)
```

## Parameters 

`string`  

The initial string to use for the cell.

## Return Value

An initialized `NSCell` object, or `nil` if the cell could not be initialized.

## Discussion

If no field editor (a shared NSText object) has been created for all `NSCell` objects, one is created.

This is one of four designated initializers you must implement when subclassing. See Designated Initializers for the complete list.

## See Also

### Initializing a Cell

init(imageCell: NSImage?)

Returns an `NSCell` object initialized with the specified image and set to have the cell’s default menu.

