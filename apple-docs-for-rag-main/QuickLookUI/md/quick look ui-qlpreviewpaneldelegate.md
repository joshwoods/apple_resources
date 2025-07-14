

- Quick Look UI
-  QLPreviewPanelDelegate 

Protocol

# QLPreviewPanelDelegate

A protocol for the delegate of the Quick Look preview panel.

macOS 12.0+

``` source
protocol QLPreviewPanelDelegate : NSWindowDelegate
```

## Overview

You can implement these methods to perform custom tasks in response to events in the preview panel.

## Topics

### Optional Methods

func previewPanel(QLPreviewPanel!, handle: NSEvent!) -> Bool

Handles an event that the preview panel receives, but doesn’t handle.

func previewPanel(QLPreviewPanel!, sourceFrameOnScreenFor: (any QLPreviewItem)!) -> NSRect

Returns the screen rectangle for a given preview item.

func previewPanel(QLPreviewPanel!, transitionImageFor: (any QLPreviewItem)!, contentRect: UnsafeMutablePointer&lt;NSRect>!) -> Any!

Returns the image to use for the transition zoom effect for a given item.

## Relationships

### Inherits From

- NSObjectProtocol
- NSWindowDelegate

## See Also

### Previews

class QLPreviewPanel

A class that implements the Quick Look preview panel to display a preview of a list of items.

class QLPreviewView

A Quick Look preview of an item that you can embed into your view hierarchy.

protocol QLPreviewItem

A protocol that defines a set of properties you implement to make a preview of your application’s content.

protocol QLPreviewPanelDataSource

A protocol that the Quick Look preview panel uses to access the contents of its data source object.

typealias QLPreviewItemLoadingBlock

A type that defines a block used to load a Quick Look preview item.

Deprecated

