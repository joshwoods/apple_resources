

- AppKit
- NSColor
-  write(to:) 

Instance Method

# write(to:)

Writes the color object’s data to the specified pasteboard.

macOS

``` source
func write(to pasteBoard: NSPasteboard)
```

## Parameters 

`pasteBoard`  

The pasteboard to which to write the receiver’s color data. If this pasteboard doesn’t support color data, the method does nothing.

## See Also

### Copying and Pasting Color Information

init?(from: NSPasteboard)

Creates a color object from color data currently on the pasteboard.

