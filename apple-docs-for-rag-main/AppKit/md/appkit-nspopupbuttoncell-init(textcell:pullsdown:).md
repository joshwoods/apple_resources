

- AppKit
- NSPopUpButtonCell
-  init(textCell:pullsDown:) 

Initializer

# init(textCell:pullsDown:)

Returns an `NSPopUpButtonCell` object initialized with the specified title.

macOS

``` source
@MainActor
init(
    textCell stringValue: String,
    pullsDown pullDown: Bool
)
```

## Parameters 

`stringValue`  

The title of the first menu. You may specify an empty string if you do not want to add an initial menu item.

`pullDown`  

true if you want the receiver to display a pull-down menu; otherwise, false if you want it to display a pop-up menu.

## Return Value

An initialized `NSPopUpButtonCell` object, or `nil` if the object could not be initialized.

## Discussion

This menu item is assigned the default pop-up button action that displays the menu. To set the action and target, use the setAction: and setTarget: methods of the item’s corresponding NSMenuItem object.

This method is the designated initializer of the class.

## See Also

### Related Documentation

Application Menu and Pop-up List Programming Topics

