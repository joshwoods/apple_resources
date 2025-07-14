

- UIKit
- UIPreviewActionGroup
-  init(title:style:actions:) Deprecated

Initializer

# init(title:style:actions:)

Creates a peek quick action group using a specified title, style, and array of peek quick actions.

iOS 9.0–13.0DeprecatediPadOS 9.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOS 9.0–13.0Deprecated

``` source
@MainActor
convenience init(
    title: String,
    style: UIPreviewAction.Style,
    actions: [UIPreviewAction]
)
```

## Parameters 

`title`  

The peek quick action group’s title

`style`  

The style for the peek quick action group.

When the system presents the group’s submenu, each child quick action is displayed using its own style. The available styles are described in the UIPreviewActionStyle enumeration in UIPreviewActionItem.

`actions`  

An array of UIPreviewAction objects, displayed as the child quick actions for the peek quick action group.

## Return Value

A newly initialized peek quick action group with your specified title, style, and submenu of peek quick actions.

