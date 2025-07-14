

- UIKit
- UIDocumentBrowserViewController
-  customActions 

Instance Property

# customActions

Custom document browser actions.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var customActions: [UIDocumentBrowserAction] { get set }
```

## Mentioned in 

Adding custom actions and activities

## Discussion

By default, this property contains an empty array. Assign an array of UIDocumentBrowserAction objects to add custom document browser actions.

Document browser actions can be accessed in two ways:

- *Navigation bar* actions appear in the Navigation bar when the user places the browser into the Select mode.

- *Menu* actions appear when the user long presses on a document or folder.

When triggered, these actions are passed the URLs of the currently selected items.

## See Also

### Adding custom actions

class UIDocumentBrowserAction

A custom action that you can create and add to a document browser’s Edit menu or navigation bar.

