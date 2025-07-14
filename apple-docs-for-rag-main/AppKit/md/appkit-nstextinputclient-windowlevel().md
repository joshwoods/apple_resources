

- AppKit
- NSTextInputClient
-  windowLevel() 

Instance Method

# windowLevel()

Returns the window level of the receiver.

macOS

``` source
optional func windowLevel() -> Int
```

## Return Value

The window level of the receiver.

## Discussion

Implementation of this method is optional. A class adopting `NSTextInputClient` can implement this interface to specify its window level if it is higher than `NSFloatingWindowLevel`.

## See Also

### Placing content

var documentVisibleRect: NSRect

var unionRectInVisibleSelectedRange: NSRect

func preferredTextAccessoryPlacement() -> NSTextCursorAccessoryPlacement

