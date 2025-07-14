

- WebKit
- WebView
-  groupName Deprecated

Instance Property

# groupName

The receiver’s group name.

macOS 10.3–10.14Deprecated

``` source
@MainActor
var groupName: String! { get set }
```

Deprecated

No longer supported; please adopt WKWebView.

## Discussion

You might use this to set the group name of a `WebView` object after it is loaded from a nib file.

## See Also

### Related Documentation

init!(frame: NSRect, frameName: String!, groupName: String!)

Initializes the receiver with a frame rectangle, frame name, and group name.

Deprecated

