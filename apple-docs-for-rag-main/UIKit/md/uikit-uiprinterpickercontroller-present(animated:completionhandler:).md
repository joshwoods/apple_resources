

- UIKit
- UIPrinterPickerController
-  present(animated:completionHandler:) 

Instance Method

# present(animated:completionHandler:)

Presents the picker from a view controller of your app.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func present(
    animated: Bool,
    completionHandler completion: UIPrinterPickerController.CompletionHandler? = nil
) -> Bool
```

## Parameters 

`animated`  

true to animate the display of the picker or false to display it without animations.

`completion`  

A block to execute when the picker is dismissed. Use this block to receive information about the selected printer or information about any errors that occurred.

## Return Value

true if the picker was displayed or false if the picker was already visible.

## Discussion

This method presents the picker from one of your app’s view controllers and returns immediately. If you provide a delegate object and that object implements the printerPickerControllerParentViewController(_:) method, UIKit uses the view controller you provide to present the picker. If you do not provide a delegate, or your delegate object does not implement the printerPickerControllerParentViewController(_:) method, UIKit presents the picker from the root view controller of your app’s main window.

After presenting the picker, the picker interface runs until the user or your app dismisses it. The picker interface provides ways for the user to cancel printing directly, all of which dismiss the picker. You can also dismiss the printer picker programmatically by calling the dismiss(animated:) method.

## See Also

### Presenting and dismissing the picker

func present(from: UIBarButtonItem, animated: Bool, completionHandler: UIPrinterPickerController.CompletionHandler?) -> Bool

Presents the picker in a popover that anchors to the specified bar button item.

func present(from: CGRect, in: UIView, animated: Bool, completionHandler: UIPrinterPickerController.CompletionHandler?) -> Bool

Presents the picker in a popover that anchors to a rectangle in the specified view.

func dismiss(animated: Bool)

Dismisses the picker.

