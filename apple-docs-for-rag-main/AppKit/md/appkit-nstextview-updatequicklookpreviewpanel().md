

- AppKit
- NSTextView
-  updateQuickLookPreviewPanel() 

Instance Method

# updateQuickLookPreviewPanel()

Notifies the QuickLook panel that an update may be required.

macOS 10.7+

``` source
@MainActor
func updateQuickLookPreviewPanel()
```

## Discussion

Notifies the QLPreviewPanel class for possible status changes with the data source or controller. Typically invoked in response to selection changes.

## See Also

### Supporting QuickLook

func toggleQuickLookPreviewPanel(Any?)

An action message that toggles the visibility state of the Quick Look preview panel.

func quickLookPreviewableItems(inRanges: [NSValue]) -> [any QLPreviewItem]

Returns an array of URLs for items that can be displayed by QuickLook in the specified ranges.

