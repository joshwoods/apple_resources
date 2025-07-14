

- AppKit
- NSBrowser
-  doubleAction 

Instance Property

# doubleAction

The browser’s double-click action method.

macOS

``` source
@MainActor
var doubleAction: Selector? { get set }
```

## See Also

### Related Documentation

func doDoubleClick(Any?)

Responds to double clicks in a column of the browser.

### Managing Actions

var sendsActionOnArrowKeys: Bool

A Boolean that indicates whether pressing an arrow key causes an action message to be sent.

func sendAction() -> Bool

Sends the action message to the target.

