

- UIKit
- UIPasteboard
-  name 

Instance Property

# name

The name of the pasteboard.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
var name: UIPasteboard.Name { get }
```

## Discussion

Names of app pasteboard objects should be unique across installed apps. If the object is a system pasteboard, this property returns one of the constants described in Pasteboard Names.

## See Also

### Related Documentation

init?(name: UIPasteboard.Name, create: Bool)

Returns a pasteboard that you identify by name, optionally creating it if it doesn’t exist.

class func withUniqueName() -> UIPasteboard

Returns an app pasteboard that you identify by a unique system-generated name.

### Getting and setting pasteboard attributes

var changeCount: Int

The number of times the pasteboard’s contents change.

