

- AppKit
-  NSDraggingInfo 

Protocol

# NSDraggingInfo

A set of methods that supply information about a dragging session.

macOS

``` source
protocol NSDraggingInfo : NSObjectProtocol
```

## Overview

You invoke the NSDraggingInfo protocol methods from within a class’s implementation of NSDraggingDestination methods. AppKit automatically passes an object that conforms to the NSDraggingInfo protocol as the argument to each of the methods that NSDraggingDestination defines. Send NSDraggingInfo messages to this object. You never need to create a class that implements the NSDraggingInfo protocol.

## Topics

### Obtaining information about the dragging session

var draggingPasteboard: NSPasteboard

The pasteboard object that holds the dragged data.

**Required**

var draggingSequenceNumber: Int

A number that uniquely identifies the dragging session.

**Required**

var draggingSource: Any?

The source, or owner, of the dragged data.

**Required**

var draggingSourceOperationMask: NSDragOperation

Information about the dragging operation and the data it contains.

**Required**

var draggingLocation: NSPoint

The current location of the mouse pointer in the base coordinate system of the destination object’s window.

**Required**

var draggingDestinationWindow: NSWindow?

The destination window for the dragging operation.

**Required**

var numberOfValidItemsForDrop: Int

The number of valid items for a drop operation.

**Required**

func namesOfPromisedFilesDropped(atDestination: URL) -> [String]?

Sets the drop location for promised files and returns the names of the files that the receiver promises to create there.

**Required**

Deprecated

### Getting image information

var draggedImageLocation: NSPoint

The current location of the dragged image’s origin, in the base coordinate system of the destination object’s window.

**Required**

var draggedImage: NSImage?

The image that represents the dragging item.

**Required**

Deprecated

### Sliding the image

func slideDraggedImage(to: NSPoint)

Slides the image to a specified location.

**Required**

var animatesToDestination: Bool

A Boolean value that indicates whether the dragging formation animates while the drag is over the destination.

**Required**

var draggingFormation: NSDraggingFormation

The formation of the dragging items while the drag is over the destination.

**Required**

### Enumerate dragged items

func enumerateDraggingItems(options: NSDraggingItemEnumerationOptions, for: NSView?, classes: [AnyClass], searchOptions: [NSPasteboard.ReadingOptionKey : Any], using: (NSDraggingItem, Int, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Enumerates through each dragging item.

**Required**

### Implementing spring-loading support

var springLoadingHighlight: NSSpringLoadingHighlight

A highlighting style for your app’s user interface to display during a spring-loading operation.

**Required**

func resetSpringLoading()

Resets a spring-loading operation to its initial state.

**Required**

### Constants

struct NSDragOperation

A group of constants that represent which operations the dragging source can perform on dragging items.

struct NSDraggingItemEnumerationOptions

A group of constants that specify options to use when enumerating dragging items.

enum NSSpringLoadingHighlight

A group of constants that indicate a highlighting style for your app’s user interface to display during a spring-loading operation.

enum NSDraggingFormation

Constants that control the visual format of multiple dragging items.

enum NSDraggingContext

Constants that specify whether a drag terminates within or outside the application.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Drop Targets

protocol NSDraggingDestination

A set of methods that the destination object (or recipient) of a dragged image must implement.

protocol NSSpringLoadingDestination

A set of methods that the destination object (or recipient) of a dragged object can implement to support spring-loading.

