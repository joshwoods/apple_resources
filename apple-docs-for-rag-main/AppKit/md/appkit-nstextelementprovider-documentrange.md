

- AppKit
- NSTextElementProvider
-  documentRange 

Instance Property

# documentRange

Describes the starting and ending locations for the document.

macOS 12.0+

``` source
var documentRange: NSTextRange { get }
```

**Required**

## Discussion

The subclass could use its own implementation of a location object conforming to NSTextRange.

