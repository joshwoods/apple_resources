

- UIKit
- Views and controls
-  Collection views 

API Collection

# Collection views

Display nested views using a configurable and highly customizable layout.

## Overview

A collection view manages an ordered set of content, such as the grid of photos in the Photos app, and presents it visually.

Collection views are a collaboration between many different objects, including:

- Cells. A cell provides the visual representation for each piece of your content.

- Layouts. A layout defines the visual arrangement of the content in the collection view.

- Your data source object. This object adopts the UICollectionViewDataSource protocol and provides the data for the collection view.

- Your delegate object. This object adopts the UICollectionViewDelegate protocol and manages user interactions with the collection view’s contents, like selection and highlighting.

- Collection view controller. You typically use a UICollectionViewController object to manage a collection view. You can use other view controllers too, but a collection view controller is required for some collection-related features to work.

## Topics

### View

class UICollectionView

An object that manages an ordered collection of data items and presents them using customizable layouts.

class UICollectionViewController

A view controller that specializes in managing a collection view.

### Data

Updating collection views using diffable data sources

Streamline the display and update of data in a collection view using a diffable data source that contains identifiers.

Implementing modern collection views

Bring compositional layouts to your app and simplify updating your user interface with diffable data sources.

Building high-performance lists and collection views

Improve the performance of lists and collections in your app with prefetching and image preparation.

class UICollectionViewDiffableDataSource

The object you use to manage data and provide cells for a collection view.

protocol UICollectionViewDataSource

The methods adopted by the object you use to manage data and provide cells for a collection view.

protocol UICollectionViewDataSourcePrefetching

A protocol that provides advance warning of the data requirements for a collection view, allowing the triggering of asynchronous data load operations.

struct NSDiffableDataSourceSnapshot

A representation of the state of the data in a view at a specific point in time.

struct NSDiffableDataSourceSectionSnapshot

A representation of the state of the data in a layout section at a specific point in time.

class UIRefreshControl

A standard control that can initiate the refreshing of a scroll view’s contents.

### Cells

class UICollectionViewCell

A single data item when that item is within the collection view’s visible bounds.

class UICollectionViewListCell

A collection view cell that provides list features and default styling.

class UICollectionReusableView

A view that defines the behavior for all cells and supplementary views presented by a collection view.

### Layouts

Implementing modern collection views

Bring compositional layouts to your app and simplify updating your user interface with diffable data sources.

Layouts

Arrange your collection view content in a highly configurable layout.

### Selection management

Changing the appearance of selected and highlighted cells

Provide visual feedback to the user about the state of a cell and the transition between states.

Selecting multiple items with a two-finger pan gesture

Accelerate user selection of multiple items using the multiselect gesture on table and collection views.

### Drag and drop

Supporting Drag and Drop in Collection Views

Initiate drags and handle drops from a collection view.

protocol UICollectionViewDragDelegate

The interface for initiating drags from a collection view.

protocol UICollectionViewDropDelegate

The interface for handling drops in a collection view.

protocol UICollectionViewDropCoordinator

An interface for coordinating your custom drop-related actions with the collection view.

class UICollectionViewDropPlaceholder

A placeholder for an item dropped on a collection view.

class UICollectionViewDropProposal

Your proposed solution for handling a drop in a collection view.

protocol UICollectionViewDropItem

The data associated with an item being dropped into the collection view.

protocol UICollectionViewDropPlaceholderContext

An object that contains information about a placeholder in the collection view.

protocol UIDataSourceTranslating

An advanced interface for managing a data source object.

class UICollectionViewPlaceholder

A placeholder for an item dragged or dropped on a collection view.

## See Also

### Container views

Autosizing Views for Localization in iOS

Add auto layout constraints to your app to achieve localizable views.

Table views

Display data in a single column of customizable rows.

class UIStackView

A streamlined interface for laying out a collection of views in either a column or a row.

class UIScrollView

A view that allows the scrolling and zooming of its contained views.

