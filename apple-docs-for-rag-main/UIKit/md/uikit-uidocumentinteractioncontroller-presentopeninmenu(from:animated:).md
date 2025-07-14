

- UIKit
- UIDocumentInteractionController
-  presentOpenInMenu(from:animated:) 

Instance Method

# presentOpenInMenu(from:animated:)

Displays a menu for opening the document and anchors that menu to the specified bar button item.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func presentOpenInMenu(
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

true if this method was able to display the menu or false if it was not.

## Discussion

This method is similar to the presentOptionsMenu(from:animated:) method, but presents a menu restricted to a list of apps capable of opening the current document. This determination is made based on the document type (as indicated by the uti property) and on the document types supported by the installed apps. To support one or more document types, an app must register those types in its `Info.plist` file using the `CFBundleDocumentTypes` key.

If there are no registered apps that support opening the document, the document interaction controller does not display a menu.

This method displays the menu asynchronously. The document interaction controller dismisses the menu automatically when the user selects an appropriate app. You can also dismiss it programmatically using the dismissMenu(animated:) method.

## See Also

### Presenting and dismissing menus

func presentOptionsMenu(from: CGRect, in: UIView, animated: Bool) -> Bool

Displays an options menu and anchors it to the specified location in the view.

func presentOptionsMenu(from: UIBarButtonItem, animated: Bool) -> Bool

Displays an options menu and anchors it to the specified bar button item.

func presentOpenInMenu(from: CGRect, in: UIView, animated: Bool) -> Bool

Displays a menu for opening the document and anchors that menu to the specified view.

func dismissMenu(animated: Bool)

Dismisses the currently active menu.

