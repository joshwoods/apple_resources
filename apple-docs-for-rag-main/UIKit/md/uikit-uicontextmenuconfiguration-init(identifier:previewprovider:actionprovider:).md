

- UIKit
- UIContextMenuConfiguration
-  init(identifier:previewProvider:actionProvider:) 

Initializer

# init(identifier:previewProvider:actionProvider:)

Creates a menu configuration object with the specified action and preview providers.

iOS 13.0+iPadOS 13.0+Mac CatalysttvOS 17.0+visionOS

``` source
@MainActor @preconcurrency
convenience init(
    identifier: (any NSCopying)? = nil,
    previewProvider: UIContextMenuContentPreviewProvider? = nil,
    actionProvider: UIContextMenuActionProvider? = nil
)
```

## Parameters 

`identifier`  

A unique identifier for the menu configuration object. If you want this method to generate a unique identifier for you, specify `nil`.

`previewProvider`  

An optional block that returns the custom view controller that you use to preview content. If you specify `nil`, UIKit uses a default preview view controller.

`actionProvider`  

An optional block that provides a contextual menu to display with the preview. If you specify `nil`, UIKit doesn’t display a contextual menu with the previewed content.

## Return Value

A new menu configuration object with the specified provider blocks.

## See Also

### Creating the menu configuration object

typealias UIContextMenuContentPreviewProvider

Returns the custom view controller to use when previewing your content.

typealias UIContextMenuActionProvider

Returns an action-based contextual menu, optionally incorporating the system-suggested actions.

