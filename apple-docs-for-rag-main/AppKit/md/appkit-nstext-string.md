

- AppKit
- NSText
-  string 

Instance Property

# string

The characters of the receiver’s text.

macOS

``` source
@MainActor
var string: String { get set }
```

## Discussion

For performance reasons, this value is the current backing store of the text object. If you want to maintain a snapshot of this as you manipulate the text storage, you should make a copy of the appropriate substring.

## See Also

### Related Documentation

Cocoa Text Architecture Guide

