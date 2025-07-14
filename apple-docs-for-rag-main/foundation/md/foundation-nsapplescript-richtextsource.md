

- Foundation
- NSAppleScript
-  richTextSource 

Instance Property

# richTextSource

Returns the syntax-highlighted source code of the receiver if the receiver has been compiled and its source code is available.

macOS 10.0+

``` source
var richTextSource: NSAttributedString? { get }
```

## Discussion

Returns `nil` otherwise. It is possible for an instance of `NSAppleScript` that has been instantiated with init(contentsOf:error:) to be a script for which the source code is not available, but is nonetheless executable.

