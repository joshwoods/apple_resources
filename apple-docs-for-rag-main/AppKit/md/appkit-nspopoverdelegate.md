

- AppKit
-  NSPopoverDelegate 

Protocol

# NSPopoverDelegate

A set of optional methods that a popover delegate can implement to provide additional or custom functionality.

macOS

``` source
protocol NSPopoverDelegate : NSObjectProtocol
```

## Overview

See NSPopover for more information on popovers in general.

## Topics

### Popover Window

func detachableWindow(for: NSPopover) -> NSWindow?

Detaches the popover creating a window containing the content.

### Popover Visibility

func popoverShouldClose(NSPopover) -> Bool

Allows a delegate to override a close request.

func popoverWillShow(Notification)

Invoked when the popover will show.

func popoverDidShow(Notification)

Invoked when the popover has been shown.

func popoverWillClose(Notification)

Invoked when the popover is about to close.

func popoverDidClose(Notification)

Invoked when the popover did close.

func popoverDidDetach(NSPopover)

Indicates that a popover has been released while it’s in an implicitly detached state.

func popoverShouldDetach(NSPopover) -> Bool

Returns a Boolean value that indicates whether a popover should detach from its positioning view and become a separate window.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Popovers

class NSPopover

A means to display additional content related to existing content on the screen.

