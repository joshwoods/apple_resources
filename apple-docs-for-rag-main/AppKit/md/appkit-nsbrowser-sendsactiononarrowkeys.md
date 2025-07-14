

- AppKit
- NSBrowser
-  sendsActionOnArrowKeys 

Instance Property

# sendsActionOnArrowKeys

A Boolean that indicates whether pressing an arrow key causes an action message to be sent.

macOS

``` source
@MainActor
var sendsActionOnArrowKeys: Bool { get set }
```

## Discussion

When the value of this property is false, pressing an arrow key scrolls the browser. When the value of this property is true, it also sends the action message specified by action.

## See Also

### Managing Actions

var doubleAction: Selector?

The browser’s double-click action method.

func sendAction() -> Bool

Sends the action message to the target.

