

- SwiftUI
- ToolbarItemPlacement
-  confirmationAction 

Type Property

# confirmationAction

The item represents a confirmation action for a modal interface.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static let confirmationAction: ToolbarItemPlacement
```

## Discussion

Use confirmation actions to receive user confirmation of a particular action. An example of a confirmation action would be an action with the label “Add” to add a new event to the calendar.

In macOS and in Mac Catalyst apps, the system places `confirmationAction` items on the trailing edge in the trailing-most position of the sheet and gain the apps accent color as a background color.

In iOS, iPadOS, and tvOS, the system places `confirmationAction` items in the same location as a primaryAction placement.

In watchOS, the system places `confirmationAction` items in the trailing edge of the navigation bar.

## See Also

### Getting placement for specific actions

static let primaryAction: ToolbarItemPlacement

The item represents a primary action.

static let secondaryAction: ToolbarItemPlacement

The item represents a secondary action.

static let cancellationAction: ToolbarItemPlacement

The item represents a cancellation action for a modal interface.

static let destructiveAction: ToolbarItemPlacement

The item represents a destructive action for a modal interface.

static let navigation: ToolbarItemPlacement

The item represents a navigation action.

