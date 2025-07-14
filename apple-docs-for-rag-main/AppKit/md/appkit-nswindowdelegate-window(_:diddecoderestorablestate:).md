

- AppKit
- NSWindowDelegate
-  window(\_:didDecodeRestorableState:) 

Instance Method

# window(\_:didDecodeRestorableState:)

Tells the delegate the window is has extracted its restorable state from a given archiver.

macOS 10.7+

``` source
@MainActor
optional func window(
    _ window: NSWindow,
    didDecodeRestorableState state: NSCoder
)
```

## Parameters 

`window`  

The window extracting its restorable state from an archive.

`state`  

The coder extracting the archive.

## Discussion

This method is called during the window’s restoreState(with:) method.

## See Also

### Managing Restorable State

func window(NSWindow, willEncodeRestorableState: NSCoder)

Tells the delegate the window is about to add its restorable state to a given archiver.

