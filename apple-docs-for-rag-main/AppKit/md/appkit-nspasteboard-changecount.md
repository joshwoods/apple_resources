

- AppKit
- NSPasteboard
-  changeCount 

Instance Property

# changeCount

The receiver’s change count.

macOS

``` source
var changeCount: Int { get }
```

## Discussion

The change count starts at zero when a client creates the receiver and becomes the first owner. The change count subsequently increments each time the pasteboard ownership changes.

The change count is also returned from clearContents() and declareTypes(_:owner:). You can therefore record the value of `changeCount` at the time that you take ownership of the pasteboard and compare it with a later value to determine whether you still have ownership.

## See Also

### Related Documentation

func clearContents() -> Int

Clears the existing contents of the pasteboard.

func declareTypes([NSPasteboard.PasteboardType], owner: Any?) -> Int

Prepares the receiver for a change in its contents by declaring the new types of data it will contain and a new owner.

### Getting Information about a Pasteboard

var name: NSPasteboard.Name

The receiver’s name.

