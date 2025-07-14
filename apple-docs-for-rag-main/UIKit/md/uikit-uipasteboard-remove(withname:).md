

- UIKit
- UIPasteboard
-  remove(withName:) 

Type Method

# remove(withName:)

Invalidates the designated app pasteboard.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
class func remove(withName pasteboardName: UIPasteboard.Name)
```

## Parameters 

`pasteboardName`  

The name of the pasteboard to be invalidated.

## Discussion

Invalidation of an app pasteboard frees up all resources used by it. Once a pasteboard is invalidated, you cannot use the it; `UIPasteboard` ignores any calls to it. The method has no effect if called with the name of a system pasteboard.

## See Also

### Getting and removing pasteboards

class var general: UIPasteboard

The systemwide general pasteboard, which you use for general copy-paste operations.

init?(name: UIPasteboard.Name, create: Bool)

Returns a pasteboard that you identify by name, optionally creating it if it doesn’t exist.

class func withUniqueName() -> UIPasteboard

Returns an app pasteboard that you identify by a unique system-generated name.

