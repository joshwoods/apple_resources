

- PencilKit
- PKToolPicker
-  shared(for:) Deprecated

Type Method

# shared(for:)

Returns the tool picker object to use for the specified window.

iOS 13.0–14.0DeprecatediPadOS 13.0–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
class func shared(for window: UIWindow) -> PKToolPicker?
```

Deprecated

Create individual instances of the tool picker using init() or init(toolItems:) instead.

## Parameters 

`window`  

A window of your app.

## Return Value

The tool picker associated with the window, or `nil` if an error occurred.

## Discussion

Call this method when you want to retrieve the tool picker assigned to one of your app’s windows. If the specified window doesn’t yet have a tool picker, this method creates and associates it with that window.

## See Also

### Deprecated

var selectedTool: any PKTool

The currently selected tool in the tool picker.

Deprecated

