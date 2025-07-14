

- UIKit
- UIPreviewAction
-  init(title:style:handler:) Deprecated

Initializer

# init(title:style:handler:)

Creates a peek quick action using a specified title, style, and handler.

iOS 9.0–13.0DeprecatediPadOS 9.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOS 9.0–13.0Deprecated

``` source
@MainActor
convenience init(
    title: String,
    style: UIPreviewAction.Style,
    handler: @escaping (UIPreviewAction, UIViewController) -> Void
)
```

## Parameters 

`title`  

The quick action’s title.

`style`  

The quick action’s style. For a complete list of styles, see the `UIPreviewActionStyle` enumeration in *UIPreviewActionItem Protocol Reference*.

`handler`  

A block that is called when the user selects the peek quick action. The block takes the following parameters:

action  
The peek quick action selected by the user.

previewViewController  
The view controller displayed as the peek.

## Return Value

A newly-created peek quick action.

## See Also

### Creating a peek quick action

var handler: (any UIPreviewActionItem, UIViewController) -> Void

The block called when the peek quick action is selected by the user.

Deprecated

enum Style

The style for a peek quick action.

Deprecated

