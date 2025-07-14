

- UIKit
-  UICollectionViewDelegate 

Protocol

# UICollectionViewDelegate

The methods adopted by the object you use to manage user interactions with items in a collection view.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
protocol UICollectionViewDelegate : UIScrollViewDelegate
```

## Overview

A collection view delegate manages user interactions with the collection view’s contents, including item selection, highlighting, and performing actions on those items. The methods of this protocol are all optional.

When configuring the collection view object, assign your delegate object to its delegate property. For more information, see UICollectionView.

## Topics

### Managing the selected cells

Changing the appearance of selected and highlighted cells

Provide visual feedback to the user about the state of a cell and the transition between states.

Selecting multiple items with a two-finger pan gesture

Accelerate user selection of multiple items using the multiselect gesture on table and collection views.

func collectionView(UICollectionView, shouldSelectItemAt: IndexPath) -> Bool

Asks the delegate if the specified item should be selected.

func collectionView(UICollectionView, didSelectItemAt: IndexPath)

Tells the delegate that the item at the specified index path was selected.

func collectionView(UICollectionView, shouldDeselectItemAt: IndexPath) -> Bool

Asks the delegate if the specified item should be deselected.

func collectionView(UICollectionView, didDeselectItemAt: IndexPath)

Tells the delegate that the item at the specified path was deselected.

func collectionView(UICollectionView, shouldBeginMultipleSelectionInteractionAt: IndexPath) -> Bool

Asks the delegate whether the user can select multiple items using a two-finger pan gesture in a collection view.

func collectionView(UICollectionView, didBeginMultipleSelectionInteractionAt: IndexPath)

Tells the delegate when the user starts using a two-finger pan gesture to select multiple items in a collection view.

func collectionViewDidEndMultipleSelectionInteraction(UICollectionView)

Tells the delegate when the user stops using a two-finger pan gesture to select multiple items in a collection view.

### Managing cell highlighting

func collectionView(UICollectionView, shouldHighlightItemAt: IndexPath) -> Bool

Asks the delegate if the item should be highlighted during tracking.

func collectionView(UICollectionView, didHighlightItemAt: IndexPath)

Tells the delegate that the item at the specified index path was highlighted.

func collectionView(UICollectionView, didUnhighlightItemAt: IndexPath)

Tells the delegate that the highlight was removed from the item at the specified index path.

### Tracking the addition and removal of views

func collectionView(UICollectionView, willDisplay: UICollectionViewCell, forItemAt: IndexPath)

Tells the delegate that the specified cell is about to be displayed in the collection view.

func collectionView(UICollectionView, willDisplaySupplementaryView: UICollectionReusableView, forElementKind: String, at: IndexPath)

Tells the delegate that the specified supplementary view is about to be displayed in the collection view.

func collectionView(UICollectionView, didEndDisplaying: UICollectionViewCell, forItemAt: IndexPath)

Tells the delegate that the specified cell was removed from the collection view.

func collectionView(UICollectionView, didEndDisplayingSupplementaryView: UICollectionReusableView, forElementOfKind: String, at: IndexPath)

Tells the delegate that the specified supplementary view was removed from the collection view.

### Handling layout changes

func collectionView(UICollectionView, transitionLayoutForOldLayout: UICollectionViewLayout, newLayout: UICollectionViewLayout) -> UICollectionViewTransitionLayout

Asks for the custom transition layout to use when moving between the specified layouts.

func collectionView(UICollectionView, targetContentOffsetForProposedContentOffset: CGPoint) -> CGPoint

Gives the delegate an opportunity to customize the content offset for layout changes and animated updates.

func collectionView(UICollectionView, targetIndexPathForMoveOfItemFromOriginalIndexPath: IndexPath, atCurrentIndexPath: IndexPath, toProposedIndexPath: IndexPath) -> IndexPath

Asks the delegate for the index path to use when moving an item.

### Managing context menus

Adding context menus in your app

Provide quick access to useful actions by adding context menus to your iOS app.

func collectionView(UICollectionView, willDisplayContextMenu: UIContextMenuConfiguration, animator: (any UIContextMenuInteractionAnimating)?)

Informs the delegate when a context menu will appear.

func collectionView(UICollectionView, willEndContextMenuInteraction: UIContextMenuConfiguration, animator: (any UIContextMenuInteractionAnimating)?)

Informs the delegate when a context menu will disappear.

func collectionView(UICollectionView, willPerformPreviewActionForMenuWith: UIContextMenuConfiguration, animator: any UIContextMenuInteractionCommitAnimating)

Informs the delegate when a user triggers a commit by tapping the preview.

func collectionView(UICollectionView, contextMenuConfigurationForItemsAt: [IndexPath], point: CGPoint) -> UIContextMenuConfiguration?

Asks the delegate for a context-menu configuration for the items at the specified index paths.

func collectionView(UICollectionView, contextMenuConfiguration: UIContextMenuConfiguration, highlightPreviewForItemAt: IndexPath) -> UITargetedPreview?

Asks the delegate for a preview of the item at the specified index path when a context-menu interaction begins.

func collectionView(UICollectionView, contextMenuConfiguration: UIContextMenuConfiguration, dismissalPreviewForItemAt: IndexPath) -> UITargetedPreview?

Asks the delegate for a preview of the item at the specified index path when a context-menu interaction ends.

### Working with focus

func collectionView(UICollectionView, canFocusItemAt: IndexPath) -> Bool

Asks the delegate whether the item at the specified index path can be focused.

func indexPathForPreferredFocusedView(in: UICollectionView) -> IndexPath?

Asks the delegate for the index path of the cell that should be focused.

func collectionView(UICollectionView, shouldUpdateFocusIn: UICollectionViewFocusUpdateContext) -> Bool

Asks the delegate whether a change in focus should occur.

func collectionView(UICollectionView, didUpdateFocusIn: UICollectionViewFocusUpdateContext, with: UIFocusAnimationCoordinator)

Tells the delegate that a focus update occurred.

func collectionView(UICollectionView, selectionFollowsFocusForItemAt: IndexPath) -> Bool

Asks the delegate whether to relate selection and focus behavior for the cell at the corresponding index path.

### Editing items

func collectionView(UICollectionView, canEditItemAt: IndexPath) -> Bool

Determines whether the specified item is editable.

### Managing actions for cells

func collectionView(UICollectionView, canPerformPrimaryActionForItemAt: IndexPath) -> Bool

Asks the delegate whether to perform a primary action for the cell at the specified index path.

func collectionView(UICollectionView, performPrimaryActionForItemAt: IndexPath)

Tells the delegate to perform the primary action for the cell at the specified index path.

### Handling scene transitions

func collectionView(UICollectionView, sceneActivationConfigurationForItemAt: IndexPath, point: CGPoint) -> UIWindowScene.ActivationConfiguration?

Returns a scene activation configuration that allows the cell to expand into a new scene.

### Controlling the spring-loading behavior

func collectionView(UICollectionView, shouldSpringLoadItemAt: IndexPath, with: any UISpringLoadedInteractionContext) -> Bool

Determines whether the spring-loading interaction effect is displayed for the specified item.

### Deprecated

func collectionView(UICollectionView, targetIndexPathForMoveFromItemAt: IndexPath, toProposedIndexPath: IndexPath) -> IndexPath

Asks the delegate for the index path to use when moving an item.

Deprecated

func collectionView(UICollectionView, contextMenuConfigurationForItemAt: IndexPath, point: CGPoint) -> UIContextMenuConfiguration?

Returns a context menu configuration for the item at a point.

Deprecated

func collectionView(UICollectionView, previewForDismissingContextMenuWithConfiguration: UIContextMenuConfiguration) -> UITargetedPreview?

Returns the destination view when dismissing a context menu.

Deprecated

func collectionView(UICollectionView, previewForHighlightingContextMenuWithConfiguration: UIContextMenuConfiguration) -> UITargetedPreview?

Returns a view to override the default preview the collection view created.

Deprecated

func collectionView(UICollectionView, shouldShowMenuForItemAt: IndexPath) -> Bool

Asks the delegate if an action menu should be displayed for the specified item.

Deprecated

func collectionView(UICollectionView, canPerformAction: Selector, forItemAt: IndexPath, withSender: Any?) -> Bool

Asks the delegate if it can perform the specified action on an item in the collection view.

Deprecated

func collectionView(UICollectionView, performAction: Selector, forItemAt: IndexPath, withSender: Any?)

Tells the delegate to perform the specified action on an item in the collection view.

Deprecated

## Relationships

### Inherits From

- NSObjectProtocol
- UIScrollViewDelegate

### Inherited By

- UICollectionViewDelegateFlowLayout

### Conforming Types

- UICollectionViewController

## See Also

### Managing collection view interactions

var delegate: (any UICollectionViewDelegate)?

The object that acts as the delegate of the collection view.

