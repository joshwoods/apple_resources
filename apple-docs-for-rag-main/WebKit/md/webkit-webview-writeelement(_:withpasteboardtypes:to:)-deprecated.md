

- WebKit
- WebView
-  writeElement(\_:withPasteboardTypes:to:) Deprecated

Instance Method

# writeElement(\_:withPasteboardTypes:to:)

Writes an element to the pasteboard using a list of types.

macOS 10.3–10.14Deprecated

``` source
@MainActor
func writeElement(
    _ element: [AnyHashable : Any]!,
    withPasteboardTypes types: [Any]!,
    to pasteboard: NSPasteboard!
)
```

Deprecated

No longer supported; please adopt WKWebView.

## Parameters 

`element`  

The element to write to the pasteboard.

`types`  

The pasteboard types to use for the element.

`pasteboard`  

The pasteboard to use for writing.

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

var pasteboardTypesForSelection: [Any]!

An array of pasteboard types that can be used for the current selection of the receiver.

Deprecated

func writeSelection(withPasteboardTypes: [Any]!, to: NSPasteboard!)

Writes the receiver’s current selection to a pasteboard using a list of types.

Deprecated

