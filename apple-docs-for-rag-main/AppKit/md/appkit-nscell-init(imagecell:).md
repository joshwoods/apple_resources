

- AppKit
- NSCell
-  init(imageCell:) 

Initializer

# init(imageCell:)

Returns an `NSCell` object initialized with the specified image and set to have the cell’s default menu.

macOS

``` source
@MainActor
init(imageCell image: NSImage?)
```

## Parameters 

`image`  

The image to use for the cell. If this parameter is `nil`, no image is set.

## Return Value

An initialized `NSCell` object, or `nil` if the cell could not be initialized.

## Discussion

This is one of four designated initializers you must implement when subclassing. See Designated Initializers for the complete list.

## See Also

### Related Documentation

Control and Cell Programming Topics

### Initializing a Cell

init(textCell: String)

Returns an NSCell object initialized with the specified string and set to have the cell’s default menu.

