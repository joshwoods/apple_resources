

- AppKit
- NSWindowDelegate
-  window(\_:willEncodeRestorableState:) 

Instance Method

# window(\_:willEncodeRestorableState:)

Tells the delegate the window is about to add its restorable state to a given archiver.

macOS 10.7+

``` source
@MainActor
optional func window(
    _ window: NSWindow,
    willEncodeRestorableState state: NSCoder
)
```

## Parameters 

`window`  

The window adding its restorable state to an archive.

`state`  

The coder creating the archive.

## Discussion

This method is called during the window’s encodeRestorableState(with:) method.

## See Also

### Managing Restorable State

func window(NSWindow, didDecodeRestorableState: NSCoder)

Tells the delegate the window is has extracted its restorable state from a given archiver.

