

- AppKit
- NSTypesetter
-  sharedSystemTypesetter 

Type Property

# sharedSystemTypesetter

Returns a shared instance of a reentrant typesetter.

macOS

``` source
class var sharedSystemTypesetter: NSTypesetter { get }
```

## Return Value

The shared system typesetter. This typesetter is reentrant.

## See Also

### Related Documentation

Text Layout Programming Guide

### Getting a typesetter

class func sharedSystemTypesetter(for: NSLayoutManager.TypesetterBehavior) -> Any

Returns a shared instance of a reentrant typesetter that implements typesetting with the specified behavior.

