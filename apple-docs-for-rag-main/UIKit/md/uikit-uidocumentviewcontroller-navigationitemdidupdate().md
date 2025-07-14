

- UIKit
- UIDocumentViewController
-  navigationItemDidUpdate() 

Instance Method

# navigationItemDidUpdate()

Provides an opportunity to customize the navigation items after the navigation bar updates.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+visionOS 1.0+

``` source
@MainActor
func navigationItemDidUpdate()
```

## Discussion

The system calls `navigationItemDidUpdate()` every time `UIDocumentViewController` makes changes to the navigation item. Customize the navigation items in this method.

This example adds buttons to the navigation bar and customizes the toolbar:

```
class EditorViewController:
        UIDocumentViewController,
        UINavigationItemRenameDelegate {

    override func navigationItemDidUpdate() {
        navigationItem.customizationIdentifier = "editorViewCustomization"
        configureCenterItemGroups()
        navigationItem.rightBarButtonItem = splitView.previewVisibilityBarButton
    }

}
```

