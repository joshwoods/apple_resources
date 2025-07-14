

- AppKit
- NSHelpManager
-  showContextHelp(for:locationHint:) 

Instance Method

# showContextHelp(for:locationHint:)

Displays the context-sensitive help for a given object at or near the point on the screen specified by a given point.

macOS

``` source
@MainActor
func showContextHelp(
    for object: Any,
    locationHint pt: NSPoint
) -> Bool
```

## Parameters 

`object`  

Object for which context-sensitive help is sought.

`pt`  

Screen location at which to display the help content; it’s usually under the cursor.

## Return Value

true when help content is successfully displayed. false if help content is not displayed (for example, when there is no context-sensitive help associated with `object`).

## See Also

### Displaying Context-Sensitive Help

func contextHelp(for: Any) -> NSAttributedString?

Returns context-sensitive help for an object.

typealias ContextHelpKey

class var isContextHelpModeActive: Bool

