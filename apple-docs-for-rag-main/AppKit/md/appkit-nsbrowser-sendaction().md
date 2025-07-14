

- AppKit
- NSBrowser
-  sendAction() 

Instance Method

# sendAction()

Sends the action message to the target.

macOS

``` source
@MainActor
func sendAction() -> Bool
```

## Return Value

true if successful; false if no target for the message could be found.

## See Also

### Related Documentation

func doDoubleClick(Any?)

Responds to double clicks in a column of the browser.

func doClick(Any?)

Responds to (single) mouse clicks in a column of the browser.

### Managing Actions

var doubleAction: Selector?

The browser’s double-click action method.

var sendsActionOnArrowKeys: Bool

A Boolean that indicates whether pressing an arrow key causes an action message to be sent.

