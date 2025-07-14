

- WebKit
- WebView
-  urlTitle(from:) Deprecated

Type Method

# urlTitle(from:)

Returns the title of a URL from the specified pasteboard.

macOS 10.3–10.14Deprecated

``` source
@MainActor
class func urlTitle(from pasteboard: NSPasteboard!) -> String!
```

Deprecated

No longer supported; please adopt WKWebView.

## Parameters 

`pasteboard`  

The pasteboard containing the URL.

## Return Value

The title of the URL on `pasteboard`. Returns `nil` if there’s no URL on `pasteboard` or the URL has no title.

## See Also

### Using the Pasteboard

class func url(from: NSPasteboard!) -> URL!

Returns a URL from the specified pasteboard.

Deprecated

func pasteboardTypes(forElement: [AnyHashable : Any]!) -> [Any]!

Returns an array of pasteboard types for an element.

Deprecated

var pasteboardTypesForSelection: [Any]!

An array of pasteboard types that can be used for the current selection of the receiver.

Deprecated

func writeElement([AnyHashable : Any]!, withPasteboardTypes: [Any]!, to: NSPasteboard!)

Writes an element to the pasteboard using a list of types.

Deprecated

func writeSelection(withPasteboardTypes: [Any]!, to: NSPasteboard!)

Writes the receiver’s current selection to a pasteboard using a list of types.

Deprecated

