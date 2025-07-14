

- AppKit
- NSWindow
-  endEditing(for:) 

Instance Method

# endEditing(for:)

Forces the field editor to give up its first responder status and prepares it for its next assignment.

macOS

``` source
@MainActor
func endEditing(for object: Any?)
```

## Parameters 

`object`  

The object that is using the window’s field editor.

## Discussion

If the field editor is the first responder, it’s made to resign that status even if its resignFirstResponder() method returns false. This registration forces the field editor to send a textDidEndEditing(_:) message to its delegate. The field editor is then removed from the view hierarchy, its delegate is set to `nil`, and it’s emptied of any text it may contain.

This method is typically invoked by the object using the field editor when it’s finished. Other objects normally change the first responder by simply using makeFirstResponder(_:), which allows a field editor or other object to retain its first responder status if, for example, the user has entered an invalid value. The endEditing(for:) method should be used only as a last resort if the field editor refuses to resign first responder status. Even in this case, you should always allow the field editor a chance to validate its text and take whatever other action it needs first. You can do this by first trying to make the `NSWindow` object the first responder:

```
if ([myWindow makeFirstResponder:myWindow]) {
    /* All fields are now valid; it’s safe to use fieldEditor:forObject:
        to claim the field editor. */
}
else {
    /* Force first responder to resign. */
    [myWindow endEditingFor:nil];
}
```

## See Also

### Related Documentation

func windowWillReturnFieldEditor(NSWindow, to: Any?) -> Any?

Tells the delegate that the field editor for a text-displaying object has been requested.

### Managing Field Editors

func fieldEditor(Bool, for: Any?) -> NSText?

Returns the window’s field editor, creating it if requested.

