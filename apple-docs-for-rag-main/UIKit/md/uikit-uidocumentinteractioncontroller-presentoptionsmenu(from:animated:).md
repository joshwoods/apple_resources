

- UIKit
- UIDocumentInteractionController
-  presentOptionsMenu(from:animated:) 

Instance Method

# presentOptionsMenu(from:animated:)

Displays an options menu and anchors it to the specified bar button item.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func presentOptionsMenu(
    from item: UIBarButtonItem,
    animated: Bool
) -> Bool
```

## Parameters 

`item`  

The bar button item to which to anchor the menu.

`animated`  

Specify true to animate the appearance of the menu or false to display it immediately.

## Return Value

true if the options menu was displayed or false if it was not. The options menu may not be displayed in cases where there are no appropriate items to include in the menu.

## Discussion

The contents of the options menu are built dynamically based on three things:

- The type of the document (as specified by the uti property)

- The set of installed apps that have registered support for opening documents

- The actions that you have indicated as supported in the document interaction controller delegate’s documentInteractionController(_:canPerformAction:) method

Options that cannot be performed on the current document are not included in the menu. For example, if the document cannot be opened by any known apps, the menu does not include options for opening it.

This method displays the options menu asynchronously. The document interaction controller dismisses the menu automatically when the user selects an appropriate option. You can also dismiss it programmatically using the dismissMenu(animated:) method.

To instead present a menu that contains only a list of apps capable of opening the current document, the presentOpenInMenu(from:animated:) method instead.

## See Also

### Presenting and dismissing menus

func presentOptionsMenu(from: CGRect, in: UIView, animated: Bool) -> Bool

Displays an options menu and anchors it to the specified location in the view.

func presentOpenInMenu(from: CGRect, in: UIView, animated: Bool) -> Bool

Displays a menu for opening the document and anchors that menu to the specified view.

func presentOpenInMenu(from: UIBarButtonItem, animated: Bool) -> Bool

Displays a menu for opening the document and anchors that menu to the specified bar button item.

func dismissMenu(animated: Bool)

Dismisses the currently active menu.

