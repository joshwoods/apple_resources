

- UIKit
- UIPrinterPickerController
-  dismiss(animated:) 

Instance Method

# dismiss(animated:)

Dismisses the picker.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func dismiss(animated: Bool)
```

## Parameters 

`animated`  

true to animate the dismissal of the picker or false to remove it without animations.

## Discussion

This method dismisses a picker that you previously presented. When using this method to dismiss a picker, the picker does not call the printerPickerControllerWillDismiss(_:) or printerPickerControllerDidDismiss(_:) methods of your delegate object.

User interactions with the picker can also dismiss the picker automatically. For example, if the user selects a printer or cancels the picker, the picker dismisses itself automatically. Use this method to dismiss a picker programmatically in response to other events in your app.

## See Also

### Presenting and dismissing the picker

func present(animated: Bool, completionHandler: UIPrinterPickerController.CompletionHandler?) -> Bool

Presents the picker from a view controller of your app.

func present(from: UIBarButtonItem, animated: Bool, completionHandler: UIPrinterPickerController.CompletionHandler?) -> Bool

Presents the picker in a popover that anchors to the specified bar button item.

func present(from: CGRect, in: UIView, animated: Bool, completionHandler: UIPrinterPickerController.CompletionHandler?) -> Bool

Presents the picker in a popover that anchors to a rectangle in the specified view.

