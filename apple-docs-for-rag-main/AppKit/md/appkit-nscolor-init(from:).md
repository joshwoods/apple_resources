

- AppKit
- NSColor
-  init(from:) 

Initializer

# init(from:)

Creates a color object from color data currently on the pasteboard.

macOS

``` source
init?(from pasteBoard: NSPasteboard)
```

## Parameters 

`pasteBoard`  

The pasteboard from which to return the color.

## Return Value

The color currently on the pasteboard or `nil` if `pasteBoard` doesn’t contain color data. The returned color’s alpha component is set to 1.0 if ignoresAlpha returns true.

## See Also

### Copying and Pasting Color Information

func write(to: NSPasteboard)

Writes the color object’s data to the specified pasteboard.

