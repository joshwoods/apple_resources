

- AppKit
- NSHelpManager
-  contextHelp(for:) 

Instance Method

# contextHelp(for:)

Returns context-sensitive help for an object.

macOS

``` source
@MainActor
func contextHelp(for object: Any) -> NSAttributedString?
```

## Parameters 

`object`  

Object for which context-sensitive help is sought.

## Return Value

Context-sensitive help content.

## See Also

### Related Documentation

func setContextHelp(NSAttributedString, for: Any)

Associates help content with an object.

### Displaying Context-Sensitive Help

func showContextHelp(for: Any, locationHint: NSPoint) -> Bool

Displays the context-sensitive help for a given object at or near the point on the screen specified by a given point.

typealias ContextHelpKey

class var isContextHelpModeActive: Bool

