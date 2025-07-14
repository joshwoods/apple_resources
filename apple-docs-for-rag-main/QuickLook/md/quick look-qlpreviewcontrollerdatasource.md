

- Quick Look
-  QLPreviewControllerDataSource 

Protocol

# QLPreviewControllerDataSource

The protocol that a data source for a preview controller needs to adopt to provide preview items to the controller.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+visionOS 1.0+

``` source
@MainActor
protocol QLPreviewControllerDataSource
```

## Overview

Besides providing a QLPreviewController with items to preview, this protocol is responsible for telling the preview controller how many items it needs to include in a preview item navigation list.

## Topics

### Providing data to a preview controller

func numberOfPreviewItems(in: QLPreviewController) -> Int

Returns the number of preview items to include in the preview navigation list.

**Required**

func previewController(QLPreviewController, previewItemAt: Int) -> any QLPreviewItem

Returns the preview item that the controller displays for the specified index.

**Required**

## See Also

### Configuring a preview controller

var dataSource: (any QLPreviewControllerDataSource)?

The preview controller’s data source.

var delegate: (any QLPreviewControllerDelegate)?

The preview controller’s delegate object.

protocol QLPreviewControllerDelegate

The protocol that a delegate of a preview controller needs to adopt to handle Quick Look previews.

