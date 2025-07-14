

- AppKit
- NSWindowDelegate
-  window(\_:shouldPopUpDocumentPathMenu:) 

Instance Method

# window(\_:shouldPopUpDocumentPathMenu:)

Asks the delegate whether the window displays the title pop-up menu in response to a Command-click or Control-click on its title.

macOS 10.5+

``` source
@MainActor
optional func window(
    _ window: NSWindow,
    shouldPopUpDocumentPathMenu menu: NSMenu
) -> Bool
```

## Parameters 

`window`  

The window whose title the user Command-clicked or Control-clicked.

`menu`  

The menu the window will display, if allowed. By default, its items are the path components of the file represented by `window`.

## Return Value

true to allow the display of the title pop-up menu; false to prevent it.

## See Also

### Related Documentation

var representedURL: URL?

The URL of the file the window represents.

