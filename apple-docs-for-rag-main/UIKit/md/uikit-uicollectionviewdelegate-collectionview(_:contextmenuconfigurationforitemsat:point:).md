

- UIKit
- UICollectionViewDelegate
-  collectionView(\_:contextMenuConfigurationForItemsAt:point:) 

Instance Method

# collectionView(\_:contextMenuConfigurationForItemsAt:point:)

Asks the delegate for a context-menu configuration for the items at the specified index paths.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 17.0+visionOS 1.0+

``` source
@MainActor
optional func collectionView(
    _ collectionView: UICollectionView,
    contextMenuConfigurationForItemsAt indexPaths: [IndexPath],
    point: CGPoint
) -> UIContextMenuConfiguration?
```

## Parameters 

`collectionView`  

The collection view containing the items.

`indexPaths`  

An array of index paths corresponding to the items the menu acts on. An empty array indicates that a person is invoking the menu from a location that doesn’t map to an item index path, like the space between cells. An array with multiple index paths indicates that a person is invoking the menu on an item in a multiple selection.

`point`  

The location of the interaction in the collection view’s coordinate space.

## Return Value

A contextual menu configuration object describing the menu to present. Returning `nil` prevents the interaction from beginning. Returning an empty configuration causes the interaction to begin, and then end with a cancellation effect. You can use this cancellation effect to indicate to people that it’s possible to present a menu from this element, but that there aren’t any actions currently available.

## Mentioned in 

Building a desktop-class iPad app

## Discussion

The system calls this method when a person invokes a context menu from the collection view. Implement this method to build a UIContextMenuConfiguration according to the index paths the system passes in to this method. The following code example shows different context-menu configurations for zero, one, and multiple index paths.

```
func collectionView(_ collectionView: UICollectionView, contextMenuConfigurationForItemsAt indexPaths: [IndexPath], point: CGPoint) -> UIContextMenuConfiguration? {
    return UIContextMenuConfiguration(actionProvider: { suggestedActions in
        if indexPaths.count == 0 {
            // Construct an empty-space menu.
            return UIMenu(children: [
                UIAction(title: "New Folder") { _ in /* Implement the action. */ }
            ])
        }
        else if indexPaths.count == 1 {
            // Construct a single-item menu.
            return UIMenu(children: [
                UIAction(title: "Copy") { _ in /* Implement the action. */ },
                UIAction(title: "Delete", attributes: .destructive) { _ in /* Implement the action. */ }
            ])
        }
        else {
            // Construct a multiple-item menu.
            return UIMenu(children: [
                UIAction(title: "New Folder With Selection") { _ in /* Implement the action. */ }
            ])
        }
    })
}
```

## See Also

### Managing context menus

Adding context menus in your app

Provide quick access to useful actions by adding context menus to your iOS app.

func collectionView(UICollectionView, willDisplayContextMenu: UIContextMenuConfiguration, animator: (any UIContextMenuInteractionAnimating)?)

Informs the delegate when a context menu will appear.

func collectionView(UICollectionView, willEndContextMenuInteraction: UIContextMenuConfiguration, animator: (any UIContextMenuInteractionAnimating)?)

Informs the delegate when a context menu will disappear.

func collectionView(UICollectionView, willPerformPreviewActionForMenuWith: UIContextMenuConfiguration, animator: any UIContextMenuInteractionCommitAnimating)

Informs the delegate when a user triggers a commit by tapping the preview.

func collectionView(UICollectionView, contextMenuConfiguration: UIContextMenuConfiguration, highlightPreviewForItemAt: IndexPath) -> UITargetedPreview?

Asks the delegate for a preview of the item at the specified index path when a context-menu interaction begins.

func collectionView(UICollectionView, contextMenuConfiguration: UIContextMenuConfiguration, dismissalPreviewForItemAt: IndexPath) -> UITargetedPreview?

Asks the delegate for a preview of the item at the specified index path when a context-menu interaction ends.

