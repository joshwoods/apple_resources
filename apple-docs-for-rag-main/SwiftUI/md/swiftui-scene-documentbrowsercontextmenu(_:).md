

- SwiftUI
- Scene
-  documentBrowserContextMenu(\_:) 

Instance Method

# documentBrowserContextMenu(\_:)

Adds to a `DocumentGroupLaunchScene` actions that accept a list of selected files as their parameter.

iOS 18.1+iPadOS 18.1+Mac Catalyst 18.1+visionOS 1.0+

``` source
@MainActor @preconcurrency
func documentBrowserContextMenu(@ViewBuilder _ menu: @escaping ([URL]?) -> some View) -> some Scene
```

## Parameters 

`menu`  

Items representing the content of the menu.

## Discussion

The actions are displayed in the document browser navigation bar when a document browser is in Select mode, and also added to context menu for the file items.

