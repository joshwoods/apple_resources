

- AppKit
- NSBrowserDelegate
-  browser(\_:shouldTypeSelectFor:withCurrentSearch:) 

Instance Method

# browser(\_:shouldTypeSelectFor:withCurrentSearch:)

Sent to the delegate to determine whether keyboard-based selection (type select) for a given event and search string should proceed.

macOS 10.5+

``` source
@MainActor
optional func browser(
    _ browser: NSBrowser,
    shouldTypeSelectFor event: NSEvent,
    withCurrentSearch searchString: String?
) -> Bool
```

## Parameters 

`browser`  

The browser.

`event`  

The keyboard event being processed.

`searchString`  

The keyboard-based selection string. It is `nil` when no keyboard-based selection has begun.

## Return Value

true to allow the selection; false to disallow it.

## See Also

### Related Documentation

var allowsTypeSelect: Bool

A Boolean that indicates whether the browser allows keystroke-based selection (type select).

### Managing Selection Behavior

func browser(NSBrowser, typeSelectStringForRow: Int, inColumn: Int) -> String?

Sent to the delegate to get the keyboard-based selection (type select) string for the specified row and column.

func browser(NSBrowser, nextTypeSelectMatchFromRow: Int, toRow: Int, inColumn: Int, for: String?) -> Int

Sent to the delegate to customize a browser’s keyboard-based selection (type select) behavior.

