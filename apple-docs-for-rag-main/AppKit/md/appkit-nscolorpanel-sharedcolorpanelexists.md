

- AppKit
- NSColorPanel
-  sharedColorPanelExists 

Type Property

# sharedColorPanelExists

Returns a Boolean value indicating whether the `NSColorPanel` has been created already.

macOS

``` source
@MainActor
class var sharedColorPanelExists: Bool { get }
```

## Return Value

true if the `NSColorPanel` has been created already; otherwise false.

## See Also

### Obtaining the Shared Color-Panel Object

class var shared: NSColorPanel

Returns the shared `NSColorPanel` instance, creating it if necessary.

