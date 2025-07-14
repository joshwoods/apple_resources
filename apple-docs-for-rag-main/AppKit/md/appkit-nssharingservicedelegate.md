

- AppKit
-  NSSharingServiceDelegate 

Protocol

# NSSharingServiceDelegate

A set of methods that you use to customize the position and animation of a share sheet, and to be notified whether the item is successfully shared.

macOS

``` source
protocol NSSharingServiceDelegate : NSObjectProtocol
```

## Overview

See NSSharingService for more information.

## Topics

### Sharing Items

func sharingService(NSSharingService, willShareItems: [Any])

Invoked when the sharing service will share the specified items.

func sharingService(NSSharingService, didShareItems: [Any])

Invoked when the sharing service has finished sharing the items.

func sharingService(NSSharingService, didFailToShareItems: [Any], error: any Error)

Invoked when the sharing service encountered an error when sharing items.

### Customizing Transition Animation

func sharingService(NSSharingService, sourceFrameOnScreenForShareItem: Any) -> NSRect

Invoked when the sharing service is performed and the sharing window is displayed, to present a transition between the original items and the sharing window.

func sharingService(NSSharingService, transitionImageForShareItem: Any, contentRect: UnsafeMutablePointer&lt;NSRect>) -> NSImage?

Invoked to allow returning a custom transition image when sharing an item.

func sharingService(NSSharingService, sourceWindowForShareItems: [Any], sharingContentScope: UnsafeMutablePointer&lt;NSSharingService.SharingContentScope>) -> NSWindow?

Returns the window that contained the share items.

enum SharingContentScope

The sharing scope constants specify the nature of the things you are sharing.

### Getting an Anchor View

func anchoringView(for: NSSharingService, showRelativeTo: UnsafeMutablePointer&lt;NSRect>, preferredEdge: UnsafeMutablePointer&lt;NSRectEdge>) -> NSView?

## Relationships

### Inherits From

- NSObjectProtocol

### Inherited By

- NSCloudSharingServiceDelegate

## See Also

### Managing the Delegate

var delegate: (any NSSharingServiceDelegate)?

Specifies the delegate of the sharing service.

