

- WebKit
- WebView
-  pasteboardTypesForSelection Deprecated

Instance Property

# pasteboardTypesForSelection

An array of pasteboard types that can be used for the current selection of the receiver.

macOS 10.3–10.14Deprecated

``` source
@MainActor
var pasteboardTypesForSelection: [Any]! { get }
```

Deprecated

No longer supported; please adopt WKWebView.

## See Also

### Using the Pasteboard

class func url(from: NSPasteboard!) -> URL!

Returns a URL from the specified pasteboard.

Deprecated

class func urlTitle(from: NSPasteboard!) -> String!

Returns the title of a URL from the specified pasteboard.

Deprecated

func pasteboardTypes(forElement: [AnyHashable : Any]!) -> [Any]!

Returns an array of pasteboard types for an element.

Deprecated

func writeElement([AnyHashable : Any]!, withPasteboardTypes: [Any]!, to: NSPasteboard!)

Writes an element to the pasteboard using a list of types.

Deprecated

func writeSelection(withPasteboardTypes: [Any]!, to: NSPasteboard!)

Writes the receiver’s current selection to a pasteboard using a list of types.

Deprecated

