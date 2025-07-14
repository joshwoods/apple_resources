

- WebKit
- WebView
-  url(from:) Deprecated

Type Method

# url(from:)

Returns a URL from the specified pasteboard.

macOS 10.3–10.14Deprecated

``` source
@MainActor
class func url(from pasteboard: NSPasteboard!) -> URL!
```

Deprecated

No longer supported; please adopt WKWebView.

## Parameters 

`pasteboard`  

The pasteboard containing a URL.

## Return Value

The URL from the specified pasteboard or `nil` if there’s no URL on `pasteboard`.

## Discussion

This method supports multiple pasteboard types including `NSRULPboardType`.

## See Also

### Using the Pasteboard

class func urlTitle(from: NSPasteboard!) -> String!

Returns the title of a URL from the specified pasteboard.

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

