

- AppKit
- NSTextView
-  toggleQuickLookPreviewPanel(\_:) 

Instance Method

# toggleQuickLookPreviewPanel(\_:)

An action message that toggles the visibility state of the Quick Look preview panel.

macOS 10.7+

``` source
@IBAction @MainActor
func toggleQuickLookPreviewPanel(_ sender: Any?)
```

## Parameters 

`sender`  

The message sender.

## Discussion

This action message toggles the visibility state of the Quick Look preview panel if the receiver is the current Quick Look controller.

## See Also

### Supporting QuickLook

func updateQuickLookPreviewPanel()

Notifies the QuickLook panel that an update may be required.

func quickLookPreviewableItems(inRanges: [NSValue]) -> [any QLPreviewItem]

Returns an array of URLs for items that can be displayed by QuickLook in the specified ranges.

