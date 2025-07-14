

- PencilKit
- PKToolPicker
-  selectedTool Deprecated

Instance Property

# selectedTool

The currently selected tool in the tool picker.

iOS 13.0–18.0DeprecatediPadOS 13.0–18.0DeprecatedMac Catalyst 13.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
var selectedTool: any PKTool { get set }
```

Deprecated

Use selectedToolItem instead.

## Discussion

This is one of the available tools associated with a PKCanvasView that adopt the PKTool protocol.

## See Also

### Deprecated

class func shared(for: UIWindow) -> PKToolPicker?

Returns the tool picker object to use for the specified window.

Deprecated

