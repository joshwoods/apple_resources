

- AppKit
- NSHelpManager
-  NSHelpManager.ContextHelpKey 

Type Alias

# NSHelpManager.ContextHelpKey

macOS

``` source
typealias ContextHelpKey = String
```

## See Also

### Displaying Context-Sensitive Help

func contextHelp(for: Any) -> NSAttributedString?

Returns context-sensitive help for an object.

func showContextHelp(for: Any, locationHint: NSPoint) -> Bool

Displays the context-sensitive help for a given object at or near the point on the screen specified by a given point.

class var isContextHelpModeActive: Bool

