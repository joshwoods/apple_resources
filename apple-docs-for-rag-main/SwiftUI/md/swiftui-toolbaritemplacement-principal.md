

- SwiftUI
- ToolbarItemPlacement
-  principal 

Type Property

# principal

The system places the item in the principal item section.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
static let principal: ToolbarItemPlacement
```

## Discussion

Principal actions are key units of functionality that receive prominent placement. For example, the location field for a web browser is a principal item.

In macOS and in Mac Catalyst apps, the system places the principal item in the center of the toolbar.

In iOS, iPadOS, and tvOS, the system places the principal item in the center of the navigation bar. This item takes precedent over a title specified through `View/navigationTitle`.

## See Also

### Getting semantic placement

static let automatic: ToolbarItemPlacement

The system places the item automatically, depending on many factors including the platform, size class, or presence of other items.

static let status: ToolbarItemPlacement

The item represents a change in status for the current context.

