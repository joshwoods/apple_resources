

- AppKit
- NSBrowserDelegate
-  browserWillScroll(\_:) 

Instance Method

# browserWillScroll(\_:)

Notifies the delegate when the browser will scroll.

macOS

``` source
@MainActor
optional func browserWillScroll(_ sender: NSBrowser)
```

## Parameters 

`sender`  

The browser sending the message.

## See Also

### Scrolling

func browserDidScroll(NSBrowser)

Notifies the delegate when the browser has scrolled.

