

- AppKit
- NSTextView
-  quickLookPreviewableItems(inRanges:) 

Instance Method

# quickLookPreviewableItems(inRanges:)

Returns an array of URLs for items that can be displayed by QuickLook in the specified ranges.

macOS 10.7+

``` source
@MainActor
func quickLookPreviewableItems(inRanges ranges: [NSValue]) -> [any QLPreviewItem]
```

## Parameters 

`ranges`  

An array of ranges.

## Return Value

Returns an array of document URLs for text attachment content, if available.

## Discussion

Each preview item must conform to the QLPreviewItem protocol.

## See Also

### Supporting QuickLook

func updateQuickLookPreviewPanel()

Notifies the QuickLook panel that an update may be required.

func toggleQuickLookPreviewPanel(Any?)

An action message that toggles the visibility state of the Quick Look preview panel.

