

- Notification Center
-  NCWidgetProviding Deprecated

Protocol

# NCWidgetProviding

The interface for customizing the appearance and behavior of a Today widget.

iOS 10.0–14.0DeprecatediPadOS 10.0–14.0DeprecatedMac Catalyst 10.0–14.0DeprecatedmacOS 10.10–11.0Deprecated

**iOS, iPadOS**

``` source
protocol NCWidgetProviding : NSObjectProtocol
```

**macOS**

``` source
protocol NCWidgetProviding : NSExtensionRequestHandling
```

Deprecated

Use WidgetKit instead.

## Overview

The `NCWidgetProviding` protocol allows customization of the appearance and behavior of a Today widget.

## Topics

### Customizing the Display

func widgetMarginInsets(forProposedMarginInsets: UIEdgeInsets) -> UIEdgeInsets

Called to let a widget accept the default margin inset values or return custom values to use instead.

func widgetActiveDisplayModeDidChange(NCWidgetDisplayMode, withMaximumSize: CGSize)

Called when the active display mode changes.

enum NCWidgetDisplayMode

The modes that can be toggled between when the user activates the More button for a widget running in iOS.

### Updating a Widget’s Contents

func widgetPerformUpdate(completionHandler: (NCUpdateResult) -> Void)

Called to give a widget an opportunity to update its contents.

enum NCUpdateResult

The result of updating a widget’s state.

### Supporting Editing

var widgetAllowsEditing: Bool

A Boolean value indicating whether the widget can be edited by users.

func widgetDidBeginEditing()

Called when a user chooses the widget’s begin editing button.

func widgetDidEndEditing()

Called when a widget’s editing session ends.

## Relationships

### Inherits From

- NSExtensionRequestHandling
- NSObjectProtocol

## See Also

### Core Widget

class NCWidgetController

An object used to specify whether a Today widget has content to display.

Deprecated

