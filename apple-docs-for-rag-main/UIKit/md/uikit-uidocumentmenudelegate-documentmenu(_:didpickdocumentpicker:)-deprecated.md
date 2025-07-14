

- UIKit
- UIDocumentMenuDelegate
-  documentMenu(\_:didPickDocumentPicker:) Deprecated

Instance Method

# documentMenu(\_:didPickDocumentPicker:)

Tells the delegate that the user has selected a document picker from the menu.

iOS 8.0–13.0DeprecatediPadOS 8.0–13.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
func documentMenu(
    _ documentMenu: UIDocumentMenuViewController,
    didPickDocumentPicker documentPicker: UIDocumentPickerViewController
)
```

**Required**

## Parameters 

`documentMenu`  

The document menu object that called this method.

`documentPicker`  

The document picker that the user selected.

## Discussion

The document menu calls this method when the user selects a document picker. Set the document picker’s delegate, and then present it.

## See Also

### Responding to user actions

func documentMenuWasCancelled(UIDocumentMenuViewController)

Tells the delegate that the user dismissed the document menu.

Deprecated

