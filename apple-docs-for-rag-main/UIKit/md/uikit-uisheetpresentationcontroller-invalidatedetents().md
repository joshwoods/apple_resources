

- UIKit
- UISheetPresentationController
-  invalidateDetents() 

Instance Method

# invalidateDetents()

Notifies the sheet to re-evaluate its detent value in the next layout pass.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
@MainActor
func invalidateDetents()
```

## Discussion

When an external input (like a captured property) to a custom detent changes, call this method to notify the sheet to re-evaluate the detent.

To animate custom detents to their new heights, call this method within animateChanges(_:).

Note

You don’t need to call this method if detents only contains system detents, or if your custom detents only use information from the passed-in context.

