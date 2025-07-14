

- Quick Look UI
-  QLPreviewItem 

Protocol

# QLPreviewItem

A protocol that defines a set of properties you implement to make a preview of your application’s content.

macOS 10.6+

``` source
protocol QLPreviewItem : NSObjectProtocol
```

## Overview

Implement the properties in this protocol to make your application’s content visible in a Quick Look preview. Use QLPreviewController to display a Quick Look preview on iOS, QLPreviewPanel and QLPreviewView on macOS.

The properties in the QLPreviewItem protocol are also declared as a category on the `NSURL` class. As a result, you can use NSURL objects directly as preview items — provided that you want to use the default titles of those items. The default title for an NSURL object is the last path component of an item’s URL. To supply custom titles for preview objects, implement a class conforming to this protocol, supplying the title with the previewItemTitle property.

## Topics

### Instance Properties

var previewItemDisplayState: Any!

The display state for the preview item.

var previewItemTitle: String!

The title to display for the preview item.

var previewItemURL: URL!

The URL of the item to preview.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Previews

class QLPreviewPanel

A class that implements the Quick Look preview panel to display a preview of a list of items.

class QLPreviewView

A Quick Look preview of an item that you can embed into your view hierarchy.

protocol QLPreviewPanelDataSource

A protocol that the Quick Look preview panel uses to access the contents of its data source object.

protocol QLPreviewPanelDelegate

A protocol for the delegate of the Quick Look preview panel.

typealias QLPreviewItemLoadingBlock

A type that defines a block used to load a Quick Look preview item.

Deprecated

