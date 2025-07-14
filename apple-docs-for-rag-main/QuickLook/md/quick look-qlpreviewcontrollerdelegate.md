

- Quick Look
-  QLPreviewControllerDelegate 

Protocol

# QLPreviewControllerDelegate

The protocol that a delegate of a preview controller needs to adopt to handle Quick Look previews.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+visionOS 1.0+

``` source
protocol QLPreviewControllerDelegate : NSObjectProtocol
```

## Overview

The delegate of a QLPreviewController object needs to adopt this protocol to:

- Provide a zoom animation for Quick Look previews.

- Specify whether your app opens a URL that the user taps in a preview.

- Respond to the opening or closing of a preview.

The methods described here are optional, but expected.

## Topics

### Responding to preview requests

func previewController(QLPreviewController, frameFor: any QLPreviewItem, inSourceView: AutoreleasingUnsafeMutablePointer&lt;UIView?>) -> CGRect

Tells the delegate that the system is about to present the preview full screen or dismiss it, and asks for information to provide a zoom effect.

func previewController(QLPreviewController, transitionImageFor: any QLPreviewItem, contentRect: UnsafeMutablePointer&lt;CGRect>) -> UIImage?

Tells the delegate that the system is about to present the preview full screen or dismiss it, and asks for information to provide a smooth transition when zooming.

func previewController(QLPreviewController, transitionViewFor: any QLPreviewItem) -> UIView?

Tells the delegate that the system is about to present the preview full screen or dismiss it, and asks for information to provide a smooth transition when zooming.

func previewControllerWillDismiss(QLPreviewController)

Tells the delegate that the preview is about to close.

func previewControllerDidDismiss(QLPreviewController)

Tells the delegate that the preview was closed.

### Responding to user actions

func previewController(QLPreviewController, shouldOpen: URL, for: any QLPreviewItem) -> Bool

Tells the delegate that the preview controller is trying to open a URL.

### Editing the content of a preview

func previewController(QLPreviewController, editingModeFor: any QLPreviewItem) -> QLPreviewItemEditingMode

Returns a value that indicates how the preview controller handles edits to the content of the previewed file.

enum QLPreviewItemEditingMode

func previewController(QLPreviewController, didUpdateContentsOf: any QLPreviewItem)

Tells the delegate that the content of a preview was updated successfully.

func previewController(QLPreviewController, didSaveEditedCopyOf: any QLPreviewItem, at: URL)

Tells the delegate that the preview item’s edited content was successfully saved to a copy at the given URL.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Configuring a preview controller

var dataSource: (any QLPreviewControllerDataSource)?

The preview controller’s data source.

protocol QLPreviewControllerDataSource

The protocol that a data source for a preview controller needs to adopt to provide preview items to the controller.

var delegate: (any QLPreviewControllerDelegate)?

The preview controller’s delegate object.

