

- UIKit
-  UIDataSourceTranslating 

Protocol

# UIDataSourceTranslating

An advanced interface for managing a data source object.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
protocol UIDataSourceTranslating : NSObjectProtocol
```

## Overview

Use the methods of this protocol to map between the positions of items and sections in your data source object and the positions of those same items and sections in your presented layout. Objects that adopt this protocol do so because the position of items in their data source object don’t always match the corresponding positions in their presented layout.

UITableView and UICollectionView adopt this protocol and use it in conjunction with drag and drop operations. For example, UITableView must account for the presence of placeholder cells, which appear as rows in the table but don’t have a corresponding entry in the data source object. Typically, you don’t adopt this protocol in your own classes.

## Topics

### Managing item positions

func presentationIndexPath(forDataSourceIndexPath: IndexPath?) -> IndexPath?

Translates an index in your data source object to the equivalent index in your presented layout.

**Required**

func dataSourceIndexPath(forPresentationIndexPath: IndexPath?) -> IndexPath?

Translates an index in your presented layout to the equivalent index in your data source object.

**Required**

### Managing section positions

func presentationSectionIndex(forDataSourceSectionIndex: Int) -> Int

Translates a section index in your data source object to the equivalent section index in your presented layout.

**Required**

func dataSourceSectionIndex(forPresentationSectionIndex: Int) -> Int

Translates a section index in your presented layout to the equivalent section index in your data source object.

**Required**

### Performing actions

func performUsingPresentationValues(() -> Void)

Performs actions on the current object using index paths that are relative to the presentation layer of that object.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- UICollectionView
- UITableView

## See Also

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

class UICollectionViewPlaceholder

A placeholder for an item dragged or dropped on a collection view.

