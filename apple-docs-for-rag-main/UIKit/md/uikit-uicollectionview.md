

- UIKit
-  UICollectionView 

Class

# UICollectionView

An object that manages an ordered collection of data items and presents them using customizable layouts.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class UICollectionView
```

## Mentioned in 

Making a view into a drop destination

Making a view into a drag source

## Overview

When you add a collection view to your user interface, your app’s main job is to manage the data associated with that collection view. The collection view gets its data from the data source object, stored in the collection view’s dataSource property. For your data source, you can use a UICollectionViewDiffableDataSource object, which provides the behavior you need to simply and efficiently manage updates to your collection view’s data and user interface. Alternatively, you can create a custom data source object by adopting the UICollectionViewDataSource protocol.

Data in the collection view is organized into individual items, which you can group into sections for presentation. An item is the smallest unit of data you want to present. For example, in a photos app, an item might be a single image. The collection view presents items onscreen using a cell, which is an instance of the UICollectionViewCell class that your data source configures and provides.

In addition to its cells, a collection view can present data using other types of views. These supplementary views can be, for example, section headers and footers that are separate from the individual cells but still convey information. Support for supplementary views is optional and defined by the collection view’s layout object, which is also responsible for defining the placement of those views.

Besides embedding a UICollectionView in your user interface, you use the methods of the collection view to ensure that the visual presentation of items matches the order in your data source object. A UICollectionViewDiffableDataSource object manages this process automatically. If you’re using a custom data source, then whenever you add, delete, or rearrange data in your collection, you use the methods of UICollectionView to insert, delete, and rearrange the corresponding cells.

You also use the collection view object to manage the selected items, although for this behavior the collection view works with its associated delegate object.

### Layouts

A layout object defines the visual arrangement of the content in the collection view. A subclass of the UICollectionViewLayout class, the layout object defines the organization and location of all cells and supplementary views inside the collection view. Although it defines their locations, the layout object doesn’t actually apply that information to the corresponding views. The collection view applies layout information to the corresponding views because the creation of cells and supplementary views involves coordination between the collection view and your data source object. The layout object is like another data source, except it provides visual information instead of item data.

You typically specify a layout object when you create a collection view, but you can also change the layout of a collection view dynamically. The layout object is stored in the collectionViewLayout property. Setting this property directly updates the layout immediately, without animating the changes. If you want to animate the changes, call the setCollectionViewLayout(_:animated:completion:) method instead.

To create an interactive transition — one that is driven by a gesture recognizer or touch events — use the startInteractiveTransition(to:completion:) method to change the layout object. That method installs an intermediate layout object, which works with your gesture recognizer or event-handling code to track the transition progress. When your event-handling code determines that the transition is finished, it calls the finishInteractiveTransition() or cancelInteractiveTransition() method to remove the intermediate layout object and install the intended target layout object.

For more information, see Layouts.

### Cells and supplementary views

The collection view’s data source object provides both the content for items and the views used to present that content. When the collection view first loads its content, it asks its data source to provide a view for each visible item. The collection view maintains a queue or list of view objects that the data source has marked for reuse. Instead of creating new views explicitly in your code, you always dequeue views.

There are two methods for dequeueing views. The one you use depends on which type of view has been requested:

- Use the dequeueReusableCell(withReuseIdentifier:for:) to get a cell for an item in the collection view.

- Use the dequeueReusableSupplementaryView(ofKind:withReuseIdentifier:for:) method to get a supplementary view requested by the layout object.

Before you call either of these methods, you must tell the collection view how to create the corresponding view if one doesn’t already exist. For this, you must register either a class or a nib file with the collection view. For example, when registering cells, you use the register(_:forCellWithReuseIdentifier:) method to register a class or the register(_:forCellWithReuseIdentifier:) method to register a nib file. As part of the registration process, you specify the reuse identifier that identifies the purpose of the view. This is the same string you use when dequeueing the view later.

After dequeueing the appropriate view in your data source method, configure its content and return it to the collection view for use. After getting the layout information from the layout object, the collection view applies it to the view and displays it.

### Data prefetching

Collection views provide two prefetching techniques you can use to improve responsiveness:

- *Cell prefetching* prepares cells in advance of the time they’re required. When a collection view requires a large number of cells simultaneously — for example, a new row of cells in grid layout — the cells are requested earlier than the time required for display. Cell rendering is therefore spread across multiple layout passes, resulting in a smoother scrolling experience. Cell prefetching is enabled by default.

- *Data prefetching* provides a mechanism whereby you’re notified of the data requirements of a collection view in advance of the requests for cells. This is useful if the content of your cells relies on an expensive data loading process, such as a network request. Assign an object that conforms to the UICollectionViewDataSourcePrefetching protocol to the prefetchDataSource property to receive notifications of when to prefetch data for cells.

### Reorder items interactively

Collection views allow you to move items around based on user interactions. Typically, the order of items in a collection view is defined by your data source. If you allow users to reorder items, you can configure a gesture recognizer to track the user’s interactions with a collection view item and update that item’s position.

To begin the interactive repositioning of an item, call the beginInteractiveMovementForItem(at:) method of the collection view. While your gesture recognizer is tracking touch events, call the updateInteractiveMovementTargetPosition(_:) method to report changes in the touch location. When you’re done tracking the gesture, call the endInteractiveMovement() or cancelInteractiveMovement() method to conclude the interactions and update the collection view.

During user interactions, the collection view invalidates its layout dynamically to reflect the current position of the item. If you do nothing, the default layout behavior repositions the items for you, but you can customize the layout animations if you want. When interactions finish, the collection view updates its data source object with the new location of the item.

The UICollectionViewController class provides a default gesture recognizer that you can use to rearrange items in its managed collection view. To install this gesture recognizer, set the installsStandardGestureForInteractiveMovement property of the collection view controller to true.

### Interface Builder attributes

The following table lists the attributes that you configure for collection views in Interface Builder.

| Attribute | Description |
|----|----|
| Items | The number of prototype cells. This property controls the specified number of prototype cells for you to configure in your storyboard. Collection views must always have at least one cell and may have multiple cells for displaying different types of content or for displaying the same content in different ways. |
| Layout | The layout object to use. Use this control to select between the UICollectionViewFlowLayout object and a custom layout object that you define.  When the flow layout is selected, you can also configure the scrolling direction for the collection view’s content and whether the flow layout has header and footer views. Enabling header and footer views adds reusable views to your storyboard that you can configure with your header and footer content. You can also create those views programmatically.  When a custom layout is selected, you must specify the UICollectionViewLayout subclass to use. |

When the Flow layout is selected, the Size inspector for the collection view contains additional attributes for configuring flow layout metrics. Use those attributes to configure the size of your cells, the size of headers and footers, the minimum spacing between cells, and any margins around each section of cells. For more information about the meaning of the flow layout metrics, see UICollectionViewFlowLayout.

### Internationalization

A collection view has no direct content of its own to internationalize. Instead, you internationalize the cells and reusable views of the collection view. For more information about internationalization, see `Localization`.

### Accessibility

A collection view has no content of its own to make accessible. If your cells and reusable views contain standard UIKit controls such as UILabel and UITextField, you can make those controls accessible. When a collection view changes its onscreen layout, it posts the layoutChanged notification.

For general information about making your interface accessible, see Accessibility for UIKit.

## Topics

### Creating a collection view

init(frame: CGRect, collectionViewLayout: UICollectionViewLayout)

Creates a collection view object with the specified frame and layout.

init?(coder: NSCoder)

Creates a collection view object from data in a given unarchiver.

### Providing the collection view data

var dataSource: (any UICollectionViewDataSource)?

The object that provides the data for the collection view.

class UICollectionViewDiffableDataSource

The object you use to manage data and provide cells for a collection view.

protocol UICollectionViewDataSource

The methods adopted by the object you use to manage data and provide cells for a collection view.

Building high-performance lists and collection views

Improve the performance of lists and collections in your app with prefetching and image preparation.

### Prefetching collection view cells and data

var isPrefetchingEnabled: Bool

A Boolean value that indicates whether cell and data prefetching are enabled.

var prefetchDataSource: (any UICollectionViewDataSourcePrefetching)?

The object that acts as the prefetching data source for the collection view, receiving notifications of upcoming cell data requirements.

protocol UICollectionViewDataSourcePrefetching

A protocol that provides advance warning of the data requirements for a collection view, allowing the triggering of asynchronous data load operations.

### Managing collection view interactions

var delegate: (any UICollectionViewDelegate)?

The object that acts as the delegate of the collection view.

protocol UICollectionViewDelegate

The methods adopted by the object you use to manage user interactions with items in a collection view.

### Creating cells

struct CellRegistration

A registration for the collection view’s cells.

func dequeueConfiguredReusableCell&lt;Cell, Item>(using: UICollectionView.CellRegistration&lt;Cell, Item>, for: IndexPath, item: Item?) -> Cell

Dequeues a configured reusable cell object.

func register(AnyClass?, forCellWithReuseIdentifier: String)

Registers a class for use in creating new collection view cells.

func register(UINib?, forCellWithReuseIdentifier: String)

Registers a nib file for use in creating new collection view cells.

func dequeueReusableCell(withReuseIdentifier: String, for: IndexPath) -> UICollectionViewCell

Dequeues a reusable cell object located by its identifier.

### Creating headers and footers

struct SupplementaryRegistration

A registration for the collection view’s supplementary views.

func dequeueConfiguredReusableSupplementary&lt;Supplementary>(using: UICollectionView.SupplementaryRegistration&lt;Supplementary>, for: IndexPath) -> Supplementary

Dequeues a configured reusable supplementary view object.

func register(AnyClass?, forSupplementaryViewOfKind: String, withReuseIdentifier: String)

Registers a class for use in creating supplementary views for the collection view.

func register(UINib?, forSupplementaryViewOfKind: String, withReuseIdentifier: String)

Registers a nib file for use in creating supplementary views for the collection view.

func dequeueReusableSupplementaryView(ofKind: String, withReuseIdentifier: String, for: IndexPath) -> UICollectionReusableView

Dequeues a reusable supplementary view located by its identifier and kind.

### Configuring the background view

var backgroundView: UIView?

The view that provides the background appearance.

### Changing the layout

var collectionViewLayout: UICollectionViewLayout

The layout used to organize the collected view’s items.

func setCollectionViewLayout(UICollectionViewLayout, animated: Bool)

Changes the collection view’s layout and optionally animates the change.

func setCollectionViewLayout(UICollectionViewLayout, animated: Bool, completion: ((Bool) -> Void)?)

Changes the collection view’s layout and notifies you when the animations complete.

func startInteractiveTransition(to: UICollectionViewLayout, completion: UICollectionView.LayoutInteractiveTransitionCompletion?) -> UICollectionViewTransitionLayout

Changes the collection view’s current layout using an interactive transition effect.

func finishInteractiveTransition()

Tells the collection view to finish an interactive transition by installing the intended target layout.

func cancelInteractiveTransition()

Tells the collection view to cancel an interactive transition and return to its original layout object.

typealias LayoutInteractiveTransitionCompletion

The completion block called at the end of an interactive transition for a collection view.

### Getting the state of the collection view

var numberOfSections: Int

The number of sections displayed by the collection view.

func numberOfItems(inSection: Int) -> Int

Fetches the count of items in the specified section.

var visibleCells: [UICollectionViewCell]

An array of visible cells currently displayed by the collection view.

### Inserting, moving, and deleting Items

func insertItems(at: [IndexPath])

Inserts new items at the specified index paths.

func moveItem(at: IndexPath, to: IndexPath)

Moves an item from one location to another in the collection view.

func deleteItems(at: [IndexPath])

Deletes the items at the specified index paths.

### Inserting, moving, and deleting sections

func insertSections(IndexSet)

Inserts new sections at the specified indexes.

func moveSection(Int, toSection: Int)

Moves a section from one location to another in the collection view.

func deleteSections(IndexSet)

Deletes the sections at the specified indexes.

### Reordering items interactively

func beginInteractiveMovementForItem(at: IndexPath) -> Bool

Initiates the interactive movement of the item at the specified index path.

func updateInteractiveMovementTargetPosition(CGPoint)

Updates the position of the item within the collection view’s bounds.

func endInteractiveMovement()

Ends interactive movement tracking and moves the target item to its new location.

func cancelInteractiveMovement()

Ends interactive movement tracking and returns the target item to its original location.

### Managing drag interactions

var dragDelegate: (any UICollectionViewDragDelegate)?

The delegate object that manages the dragging of items from the collection view.

protocol UICollectionViewDragDelegate

The interface for initiating drags from a collection view.

var hasActiveDrag: Bool

A Boolean value that indicates whether items were lifted from the collection view and have not yet been dropped.

var dragInteractionEnabled: Bool

A Boolean value that indicates whether the collection view supports dragging content.

### Managing drop interactions

var dropDelegate: (any UICollectionViewDropDelegate)?

The delegate object that manages the dropping of items into the collection view.

protocol UICollectionViewDropDelegate

The interface for handling drops in a collection view.

var hasActiveDrop: Bool

A Boolean value that indicates whether the collection view is currently tracking a drop session.

var reorderingCadence: UICollectionView.ReorderingCadence

The speed at which items in the collection view are reordered to show potential drop locations.

enum ReorderingCadence

Constants indicating the speed at which collection view items are reorganized during a drop.

### Selecting cells

var indexPathsForSelectedItems: [IndexPath]?

The index paths for the selected items.

func selectItem(at: IndexPath?, animated: Bool, scrollPosition: UICollectionView.ScrollPosition)

Selects the item at the specified index path and optionally scrolls it into view.

func deselectItem(at: IndexPath, animated: Bool)

Deselects the item at the specified index.

var allowsSelection: Bool

A Boolean value that indicates whether users can select items in the collection view.

var allowsMultipleSelection: Bool

A Boolean value that determines whether users can select more than one item in the collection view.

var allowsSelectionDuringEditing: Bool

A Boolean value that determines whether users can select cells while the collection view is in editing mode.

var allowsMultipleSelectionDuringEditing: Bool

A Boolean value that controls whether users can select more than one cell simultaneously in editing mode.

var selectionFollowsFocus: Bool

A Boolean value that triggers an automatic selection when focus moves to a cell.

### Putting the collection view into edit mode

var isEditing: Bool

A Boolean value that determines whether the collection view is in editing mode.

### Locating items and views in the collection view

func indexPathForItem(at: CGPoint) -> IndexPath?

Gets the index path of the item at the specified point in the collection view.

var indexPathsForVisibleItems: [IndexPath]

An array of the visible items in the collection view.

func indexPath(for: UICollectionViewCell) -> IndexPath?

Gets the index path of the specified cell.

func cellForItem(at: IndexPath) -> UICollectionViewCell?

Gets the cell object at the index path you specify.

func indexPathsForVisibleSupplementaryElements(ofKind: String) -> [IndexPath]

Gets the index paths of all visible supplementary views of the specified type.

func supplementaryView(forElementKind: String, at: IndexPath) -> UICollectionReusableView?

Gets the supplementary view at the specified index path.

func visibleSupplementaryViews(ofKind: String) -> [UICollectionReusableView]

Gets an array of the visible supplementary views of the specified kind.

### Getting layout information

func layoutAttributesForItem(at: IndexPath) -> UICollectionViewLayoutAttributes?

Gets the layout information for the item at the specified index path.

func layoutAttributesForSupplementaryElement(ofKind: String, at: IndexPath) -> UICollectionViewLayoutAttributes?

Gets the layout information for the specified supplementary view.

### Scrolling an item into view

func scrollToItem(at: IndexPath, at: UICollectionView.ScrollPosition, animated: Bool)

Scrolls the collection view contents until the specified item is visible.

struct ScrollPosition

Constants that indicate how to scroll an item into the visible portion of the collection view.

enum ScrollDirection

Constants that indicate the direction of scrolling for the layout.

### Animating multiple changes to the collection view

func performBatchUpdates((() -> Void)?, completion: ((Bool) -> Void)?)

Animates multiple insert, delete, reload, and move operations as a group.

### Reloading content

var hasUncommittedUpdates: Bool

A Boolean value that indicates whether the collection view contains drop placeholders or is reordering its items as part of handling a drop.

func reconfigureItems(at: [IndexPath])

Updates the data for the items at the index paths you specify, preserving the existing cells for the items.

func reloadData()

Reloads all of the data for the collection view.

func reloadSections(IndexSet)

Reloads the data in the specified sections of the collection view.

func reloadItems(at: [IndexPath])

Reloads just the items at the specified index paths.

### Identifying collection view elements

enum ElementCategory

Constants specifying the type of view.

class let elementKindSectionFooter: String

A supplementary view that identifies the footer for a given section.

class let elementKindSectionHeader: String

A supplementary view that identifies the header for a given section.

### Working with focus

var allowsFocus: Bool

A Boolean value that determines whether the collection view allows its cells to become focused.

var allowsFocusDuringEditing: Bool

A Boolean value that determines whether the collection view allows its cells to become focused in edit mode.

var selectionFollowsFocus: Bool

A Boolean value that triggers an automatic selection when focus moves to a cell.

var remembersLastFocusedIndexPath: Bool

A Boolean value that indicates whether the collection view automatically assigns the focus to the item at the last focused index path.

### Managing context menus

var contextMenuInteraction: UIContextMenuInteraction?

The collection view’s context menu interaction.

### Resizing self-sizing cells

var selfSizingInvalidation: UICollectionView.SelfSizingInvalidation

The mode that the collection view uses for invalidating the size of self-sizing cells.

enum SelfSizingInvalidation

Constants that describe modes for invalidating the size of self-sizing collection view cells.

### Instance Methods

func indexPath(forSupplementaryView: UICollectionReusableView) -> IndexPath?

## Relationships

### Inherits From

- UIScrollView

### Conforms To

- CALayerDelegate
- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSTouchBarProvider
- Sendable
- UIAccessibilityIdentification
- UIActivityItemsConfigurationProviding
- UIAppearance
- UIAppearanceContainer
- UICoordinateSpace
- UIDataSourceTranslating
- UIDynamicItem
- UIFocusEnvironment
- UIFocusItem
- UIFocusItemContainer
- UIFocusItemScrollableContainer
- UILargeContentViewerItem
- UIPasteConfigurationSupporting
- UIPopoverPresentationControllerSourceItem
- UIResponderStandardEditActions
- UISpringLoadedInteractionSupporting
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### View

class UICollectionViewController

A view controller that specializes in managing a collection view.

