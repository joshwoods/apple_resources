

- AppKit
- NSPopUpButton
-  setTitle(\_:) 

Instance Method

# setTitle(\_:)

Sets the string displayed in the receiver when the user isn’t pressing the mouse button.

macOS

``` source
@MainActor
func setTitle(_ string: String)
```

## Parameters 

`string`  

The string to display.

## Discussion

If the receiver displays a pop-up menu, this method changes the current item to be the item with the specified title, adding a new item by that name if one does not already exist. If the receiver displays a pull-down list, this method sets its title to the specified string.

