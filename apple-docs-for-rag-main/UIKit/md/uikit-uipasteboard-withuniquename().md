

- UIKit
- UIPasteboard
-  withUniqueName() 

Type Method

# withUniqueName()

Returns an app pasteboard that you identify by a unique system-generated name.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
class func withUniqueName() -> UIPasteboard
```

## Return Value

An app pasteboard object with a unique name.

## Discussion

Obtain the value of the name property to discover the name of the returned pasteboard. App pasteboards returned by this method are not persistent, existing only until the app quits. Starting in iOS 10, persistent named pasteboards are deprecated. Instead use a shared container, as described in the overview for the UIPasteboard class.

## See Also

### Getting and removing pasteboards

class var general: UIPasteboard

The systemwide general pasteboard, which you use for general copy-paste operations.

init?(name: UIPasteboard.Name, create: Bool)

Returns a pasteboard that you identify by name, optionally creating it if it doesn’t exist.

class func remove(withName: UIPasteboard.Name)

Invalidates the designated app pasteboard.

