

- WebKit
- WebView
-  pasteboardTypes(forElement:) Deprecated

Instance Method

# pasteboardTypes(forElement:)

Returns an array of pasteboard types for an element.

macOS 10.3–10.14Deprecated

``` source
@MainActor
func pasteboardTypes(forElement element: [AnyHashable : Any]!) -> [Any]!
```

Deprecated

No longer supported; please adopt WKWebView.

## Parameters 

`element`  

The element whose pasteboard types you want.

## Return Value

An array of pasteboard types for an element.

## See Also

### Using the Pasteboard

class func url(from: NSPasteboard!) -> URL!

Returns a URL from the specified pasteboard.

Deprecated

class func urlTitle(from: NSPasteboard!) -> String!

Returns the title of a URL from the specified pasteboard.

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

