

- SwiftUI
- ToolbarItemPlacement
-  navigation 

Type Property

# navigation

The item represents a navigation action.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
static let navigation: ToolbarItemPlacement
```

## Discussion

Navigation actions allow the user to move between contexts. For example, the forward and back buttons of a web browser are navigation actions.

In macOS and in Mac Catalyst apps, the system places navigation items in the leading edge of the toolbar ahead of the inline title if that is present in the toolbar.

In iOS, iPadOS, and tvOS, navigation items appear in the leading edge of the navigation bar. If a system navigation item such as a back button is present in a compact width, it instead appears in the primaryAction placement.

## See Also

### Getting placement for specific actions

static let primaryAction: ToolbarItemPlacement

The item represents a primary action.

static let secondaryAction: ToolbarItemPlacement

The item represents a secondary action.

static let confirmationAction: ToolbarItemPlacement

The item represents a confirmation action for a modal interface.

static let cancellationAction: ToolbarItemPlacement

The item represents a cancellation action for a modal interface.

static let destructiveAction: ToolbarItemPlacement

The item represents a destructive action for a modal interface.

