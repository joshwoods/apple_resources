

- AppKit
- NSPDFPanel
-  beginSheet(with:modalFor:completionHandler:) 

Instance Method

# beginSheet(with:modalFor:completionHandler:)

Presents a document-modal PDF panel.

macOS 10.9+

``` source
@MainActor
func beginSheet(
    with pdfInfo: NSPDFInfo,
    modalFor docWindow: NSWindow?,
    completionHandler: @escaping (Int) -> Void
)
```

``` source
@MainActor
func beginSheet(
    with pdfInfo: NSPDFInfo,
    modalFor docWindow: NSWindow?
) async -> Int
```

## Parameters 

`pdfInfo`  

The `NSPDFInfo` object describing the parameters to be used when creating the PDF file.

`docWindow`  

The window in which the PDF panel will be presented.

`completionHandler`  

The block called when the user dismisses the PDF panel.

## Discussion

This method presents a slightly different PDF panel depending on whether the requestsParentDirectory constant is set. If the user dismisses the panel without canceling it, this method updates the NSPDFInfo object with any changes the user makes.

