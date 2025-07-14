

- AppKit
- NSOutlineViewDelegate
-  outlineViewItemWillExpand(\_:) 

Instance Method

# outlineViewItemWillExpand(\_:)

Invoked when `notification` is posted—that is, whenever the user is about to expand an item in the outline view.

macOS 10.10+

``` source
@MainActor
optional func outlineViewItemWillExpand(_ notification: Notification)
```

## Parameters 

`notification`  

The posted notification.

## Discussion

This method is invoked as a result of posting an itemWillExpandNotification.

## See Also

### Working with the Outline Column

func outlineViewColumnDidMove(Notification)

Invoked whenever the user moves a column in the outline view.

func outlineViewColumnDidResize(Notification)

Invoked whenever the user resizes a column in the outline view.

func outlineViewItemDidExpand(Notification)

Invoked when `notification` is posted—that is, whenever the user expands an item in the outline view.

func outlineViewItemWillCollapse(Notification)

Invoked when `notification` is posted—that is, whenever the user is about to collapse an item in the outline view.

func outlineViewItemDidCollapse(Notification)

Invoked when the did collapse notification is posted—that is, whenever the user collapses an item in the outline view.

