

- UIKit
-  UISheetPresentationControllerDelegate 

Protocol

# UISheetPresentationControllerDelegate

The interface that an object implements to respond to size changes in a sheet presentation controller.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
@MainActor
protocol UISheetPresentationControllerDelegate : UIAdaptivePresentationControllerDelegate
```

## Topics

### Resizing the Sheet Presentation Controller

func sheetPresentationControllerDidChangeSelectedDetentIdentifier(UISheetPresentationController)

Provides an opportunity to respond after the sheet presentation controller’s selected detent changes.

## Relationships

### Inherits From

- NSObjectProtocol
- UIAdaptivePresentationControllerDelegate

## See Also

### Managing the delegate

var delegate: (any UISheetPresentationControllerDelegate)?

The delegate of the sheet presentation controller.

