

- Foundation
- NSAppleScript
-  source 

Instance Property

# source

The script source for the receiver.

Mac Catalyst 13.0+macOS 10.0+

``` source
var source: String? { get }
```

## Discussion

It is possible for an `NSAppleScript` that has been instantiated with init(contentsOf:error:) to be a script for which the source code is not available but is nonetheless executable.

## See Also

### Getting Information About a Script

var isCompiled: Bool

A Boolean value that indicates whether the receiver’s script has been compiled.

