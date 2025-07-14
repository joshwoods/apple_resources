

- UIKit
-  UITableViewController 

Class

# UITableViewController

A view controller that specializes in managing a table view.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class UITableViewController
```

## Mentioned in 

Filling a table with data

Handling row selection in a table view

Displaying and managing views with a view controller

## Overview

Subclass UITableViewController when your interface consists of a table view and little or no other content. Table view controllers already adopt the protocols you need to manage your table view’s content and respond to changes. In addition, UITableViewController implements the following behaviors:

- Automatically loads the table view archived in a storyboard or nib file, which you can access using the tableView property

- Sets the data source and the delegate of the table view to `self`

- Implements the viewWillAppear(_:) method, automatically reloads the data for its table view on first appearance, and clears its selection (with or without animation, depending on the request) every time the table view appears (disable this last behavior by changing the value of clearsSelectionOnViewWillAppear)

- Implements the viewDidAppear(_:) method and automatically flashes the table view’s scroll indicators when it first appears

- Implements the setEditing(_:animated:) method and automatically toggles the edit mode of the table when the user taps an Edit\|Done button in the navigation bar

- Automatically resizes its table view to accommodate the appearance or disappearance of the onscreen keyboard

Create a custom subclass of UITableViewController for each table view that you manage. When you initialize the table view controller, you must specify the style of the table view (plain or grouped). You must also override the data source and delegate methods required to fill your table with data. You may override loadView() or any other superclass method, but if you do, be sure to invoke the superclass implementation of the method, usually as the first method call.

## Topics

### Creating a table view controller

init(style: UITableView.Style)

Initializes a table view controller to manage a table view of a given style.

init(nibName: String?, bundle: Bundle?)

Creates a table view controller with the nib file in the specified bundle.

init?(coder: NSCoder)

Creates a table view controller from data in an unarchiver.

### Getting the table view

var tableView: UITableView!

Returns the table view managed by the controller object.

### Configuring the table behavior

var clearsSelectionOnViewWillAppear: Bool

A Boolean value indicating if the controller clears the selection when the table appears.

### Refreshing the table view

var refreshControl: UIRefreshControl?

The refresh control used to update the table contents.

## Relationships

### Inherits From

- UIViewController

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSExtensionRequestHandling
- NSObjectProtocol
- NSTouchBarProvider
- Sendable
- UIActivityItemsConfigurationProviding
- UIAppearanceContainer
- UIContentContainer
- UIFocusEnvironment
- UIPasteConfigurationSupporting
- UIResponderStandardEditActions
- UIScrollViewDelegate
- UIStateRestoring
- UITableViewDataSource
- UITableViewDelegate
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### Content view controllers

Displaying and managing views with a view controller

Build a view controller in storyboards, configure it with custom views, and fill those views with your app’s data.

Showing and hiding view controllers

Display view controllers using different techniques, and pass data between them during transitions.

class UIViewController

An object that manages a view hierarchy for your UIKit app.

class UICollectionViewController

A view controller that specializes in managing a collection view.

protocol UIContentContainer

A set of methods for adapting the contents of your view controllers to size and trait changes.

