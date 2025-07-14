

- AppKit
- NSHelpManager
-  isContextHelpModeActive 

Type Property

# isContextHelpModeActive

macOS

``` source
@MainActor
class var isContextHelpModeActive: Bool { get set }
```

## See Also

### Displaying Context-Sensitive Help

func contextHelp(for: Any) -> NSAttributedString?

Returns context-sensitive help for an object.

func showContextHelp(for: Any, locationHint: NSPoint) -> Bool

Displays the context-sensitive help for a given object at or near the point on the screen specified by a given point.

typealias ContextHelpKey

