

- UIKit
- UIPasteboard
-  general 

Type Property

# general

The systemwide general pasteboard, which you use for general copy-paste operations.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
class var general: UIPasteboard { get }
```

## Return Value

A shared system pasteboard object with the name of general.

## Discussion

You may use the general pasteboard for copying and pasting text, images, URLs, colors, and other data within an app or between apps. The general pasteboard is persistent across device restarts and app uninstalls.

## See Also

### Getting and removing pasteboards

init?(name: UIPasteboard.Name, create: Bool)

Returns a pasteboard that you identify by name, optionally creating it if it doesn’t exist.

class func withUniqueName() -> UIPasteboard

Returns an app pasteboard that you identify by a unique system-generated name.

class func remove(withName: UIPasteboard.Name)

Invalidates the designated app pasteboard.

