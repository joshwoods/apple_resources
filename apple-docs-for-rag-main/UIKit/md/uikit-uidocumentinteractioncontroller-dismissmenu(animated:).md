

- UIKit
- UIDocumentInteractionController
-  dismissMenu(animated:) 

Instance Method

# dismissMenu(animated:)

Dismisses the currently active menu.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func dismissMenu(animated: Bool)
```

## Parameters 

`animated`  

Specify true to animate the dismissal of the currently active menu or false to dismiss it immediately.

## Discussion

Use this method to dismiss a menu programmatically. The document interaction controller can also dismiss the menu automatically in response to user actions.

## See Also

### Presenting and dismissing menus

func presentOptionsMenu(from: CGRect, in: UIView, animated: Bool) -> Bool

Displays an options menu and anchors it to the specified location in the view.

func presentOptionsMenu(from: UIBarButtonItem, animated: Bool) -> Bool

Displays an options menu and anchors it to the specified bar button item.

func presentOpenInMenu(from: CGRect, in: UIView, animated: Bool) -> Bool

Displays a menu for opening the document and anchors that menu to the specified view.

func presentOpenInMenu(from: UIBarButtonItem, animated: Bool) -> Bool

Displays a menu for opening the document and anchors that menu to the specified bar button item.

