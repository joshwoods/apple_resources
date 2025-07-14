

- ReplayKit
-  RPPreviewViewControllerDelegate 

Protocol

# RPPreviewViewControllerDelegate

The protocol you implement to respond to changes to a screen-recording user interface.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 11.0+tvOS 10.0+visionOS 1.0+

``` source
protocol RPPreviewViewControllerDelegate : NSObjectProtocol
```

## Overview

Use this class to respond to changes to a screen-recording user interface, represented by an RPBroadcastActivityViewController object.

## Topics

### Dismissing the View Controller

func previewControllerDidFinish(RPPreviewViewController)

Indicates that the preview view controller is ready to be dismissed.

func previewController(RPPreviewViewController, didFinishWithActivityTypes: Set&lt;String>)

Indicates that the preview view controller is ready to be dismissed with associated activity types.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Displaying the Preview UI

var mode: RPPreviewViewControllerMode

The type of screen that appears when the view is presented.

enum RPPreviewViewControllerMode

The modes used to determine whether the preview view controller or the share screen appears when editing a replay.

var previewControllerDelegate: (any RPPreviewViewControllerDelegate)?

The preview view controller’s delegate.

