

- AppKit
- NSApplication
-  orderedWindows 

Instance Property

# orderedWindows

An array of window objects arranged according to their front-to-back ordering on the screen.

macOS

``` source
@MainActor
var orderedWindows: [NSWindow] { get }
```

## Discussion

Only windows that are typically scriptable are included in the array. For example, panels are not included. This property is accessed during script command evaluation—for example, while finding the window in the script statement `close the second window`. For information on how your app can return its own array of ordered windows, see application:delegateHandlesKey:.

## See Also

### Scripting Your App

var orderedDocuments: [NSDocument]

An array of document objects arranged according to the front-to-back ordering of their associated windows.

