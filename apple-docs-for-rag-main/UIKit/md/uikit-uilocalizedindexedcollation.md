

- UIKit
-  UILocalizedIndexedCollation 

Class

# UILocalizedIndexedCollation

An object that organizes, sorts, and localizes the data for a table view that has a section index.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class UILocalizedIndexedCollation
```

## Overview

Use a UILocalizedIndexedCollation object in conjunction with your table’s data source object to sort and manage the data in an indexed table view. An index is an ideal way for users to navigate a table view containing sequential content. For example, the Contacts app sorts contacts alphabetically and displays an index for navigating those contacts quickly. You use the collation object as the source of the table’s section titles and index titles in your table view. You also use it to sort items in each section of your table.

To prepare the data for a section index, create an indexed-collation object and call section(for:collationStringSelector:) for each model object to be indexed. That method determines the section in which each of these objects should appear and returns an integer that identifies the section. The table-view controller then puts each object in a local array for its section. For each section array, the controller calls the sortedArray(from:collationStringSelector:) method to sort all of the objects in the section. The indexed-collation object is now the data store that the table-view controller uses to provide section-index data to the table view, as shown in the following example code.

- Swift
- Objective-C

```
func tableView(tableView: UITableView!, titleForHeaderInSection section: Int) -> String! {
    let currentCollation = UILocalizedIndexedCollation.currentCollation() as UILocalizedIndexedCollation
    let sectionTitles = currentCollation.sectionTitles as NSArray
    return sectionTitles.objectAtIndex(section) as String
}

func sectionIndexTitlesForTableView(tableView: UITableView!) -> NSArray! {
    let currentCollation = UILocalizedIndexedCollation.currentCollation() as UILocalizedIndexedCollation
    return currentCollation.sectionIndexTitles as NSArray
}

func tableView(tableView: UITableView!, sectionForSectionIndexTitle title: String!, atIndex index: Int) -> Int {
    let currentCollation = UILocalizedIndexedCollation.currentCollation() as UILocalizedIndexedCollation
    return currentCollation.sectionForSectionIndexTitleAtIndex(index)
}
```

```
- (NSString *)tableView:(UITableView *)tableView titleForHeaderInSection:(NSInteger)section
{
    return [[[UILocalizedIndexedCollation currentCollation] sectionTitles] objectAtIndex:section];
}

- (NSArray *)sectionIndexTitlesForTableView:(UITableView *)tableView
{
    return [[UILocalizedIndexedCollation currentCollation] sectionIndexTitles];
}

- (NSInteger)tableView:(UITableView *)tableView sectionForSectionIndexTitle:(NSString *)title atIndex:(NSInteger)index
{
    return [[UILocalizedIndexedCollation currentCollation] sectionForSectionIndexTitleAtIndex:index];
}
```

## Topics

### Getting the shared instance

class func current() -> Self

Returns an indexed-collation instance for the current table view.

### Preparing the sections and section indexes

func section(for: Any, collationStringSelector: Selector) -> Int

Returns an integer identifying the section in which a model object belongs.

func sortedArray(from: [Any], collationStringSelector: Selector) -> [Any]

Sorts the objects within a section by their localized titles.

### Providing section index data to the table view

var sectionTitles: [String]

Returns the list of section titles for the table view.

var sectionIndexTitles: [String]

Returns the list of section-index titles for the table view.

func section(forSectionIndexTitle: Int) -> Int

Returns the section that the table view should scroll to for the given index title.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Data

Filling a table with data

Create and configure cells for your table dynamically using a data source object, or provide them statically from your storyboard.

Asynchronously loading images into table and collection views

Store and fetch images asynchronously to make your app more responsive.

protocol UITableViewDataSource

The methods that an object adopts to manage data and provide cells for a table view.

protocol UITableViewDataSourcePrefetching

A protocol that provides advance warning of the data requirements for a table view, allowing you to start potentially long-running data operations early.

class UITableViewDiffableDataSource

The object you use to manage data and provide cells for a table view.

struct NSDiffableDataSourceSnapshot

A representation of the state of the data in a view at a specific point in time.

protocol UIDataSourceTranslating

An advanced interface for managing a data source object.

class UIRefreshControl

A standard control that can initiate the refreshing of a scroll view’s contents.

