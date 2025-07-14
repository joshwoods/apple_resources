

- AppKit
- NSWindowDelegate
-  windowWillReturnFieldEditor(\_:to:) 

Instance Method

# windowWillReturnFieldEditor(\_:to:)

Tells the delegate that the field editor for a text-displaying object has been requested.

macOS

``` source
@MainActor
optional func windowWillReturnFieldEditor(
    _ sender: NSWindow,
    to client: Any?
) -> Any?
```

## Parameters 

`sender`  

The window requesting the field editor from the delegate.

`client`  

A text-displaying object to be associated with the field editor. If `nil`, the requested field editor is the default.

## Return Value

The field editor for `client`; returns `nil` when the delegate has no field editor to assign.

## See Also

### Related Documentation

func fieldEditor(Bool, for: Any?) -> NSText?

Returns the window’s field editor, creating it if requested.

