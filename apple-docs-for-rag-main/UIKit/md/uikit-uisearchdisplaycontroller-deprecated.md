

- UIKit
-  UISearchDisplayController Deprecated

Class

# UISearchDisplayController

An object that manages the display of a search bar, along with a table view that displays search results.

iOS 3.0–8.0DeprecatediPadOS 3.0–8.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
class UISearchDisplayController
```

Deprecated

Use UISearchController instead.

## Overview

You initialize a search display controller with a search bar and a view controller responsible for managing the data to be searched. When the user starts a search, the search display controller superimposes the search interface over the original view controller’s view and shows the search results in its table view.

In addition to managing the searchable data, the original view controller typically plays four more roles you need to fill when using a search display controller. Those roles are the following:

1.  Data source for the search results table view (searchResultsDataSource), which provides the data for the results table.

2.  Delegate for the search results table view (searchResultsDelegate), which responds to the user’s selection of an item in the results table.

3.  Delegate for the search display controller (delegate), which responds to events such the starting or ending of a search, and the showing or hiding of the search interface. As a convenience, this delegate may also be told about changes to the search string or search scope, so that the results table view can be reloaded.

4.  Delegate for the search bar (delegate described in UISearchBar), which responds to changes in search criteria.

Typically, you initialize a search display controller from a view controller (usually an instance of UITableViewController) that’s displaying a list. See the Simple UISearchBar with State Restoration sample code project for an example of how to configure a search display controller in Interface Builder. To perform configuration programmatically, set `self` for the search display controller’s view controller and search results data source and delegate, as shown here:

```
searchController = [[UISearchDisplayController alloc]
                         initWithSearchBar:searchBar contentsController:self];
searchController.delegate = self;
searchController.searchResultsDataSource = self;
searchController.searchResultsDelegate = self;
```

If you follow this pattern, then in the table view data source and delegate methods you can check the methods’ table view argument to determine which table view is sending the message:

```
- (NSInteger)tableView:(UITableView *)tableView numberOfRowsInSection:(NSInteger)section {

    if (tableView == self.tableView) {
        return ...;
    }
    // If necessary (if self is the data source for other table views),
    // check whether tableView is searchController.searchResultsTableView.
    return ...;
}
```

Important

A view controller or search bar can be associated with only a single search display controller at a time. If a search display controller is destroyed (for example, in response to a memory warning), then you can create a new one and associate it with the original view controller or search bar.

Starting in iOS 7.0, you can use a search display controller with a navigation bar (an instance of the UINavigationBar class) by configuring the search display controller’s displaysSearchBarInNavigationBar and navigationItem properties.

## Topics

### Initializing a search bar

init(searchBar: UISearchBar, contentsController: UIViewController)

Returns a display controller initialized with the given search bar and contents controller.

### Displaying the search Interface

var isActive: Bool

The visibility state of the search interface.

func setActive(Bool, animated: Bool)

Displays or hides the search interface, optionally with animation.

### Configuring a search bar

var delegate: (any UISearchDisplayDelegate)?

The controller’s delegate.

var searchBar: UISearchBar

The search bar.

var searchContentsController: UIViewController

The view controller that manages the contents being searched.

var searchResultsTableView: UITableView

The table view in which the search results are displayed.

var searchResultsDataSource: (any UITableViewDataSource)?

The data source for the table view in which the search results are displayed.

var searchResultsDelegate: (any UITableViewDelegate)?

The delegate for the table view in which the search results are displayed.

var searchResultsTitle: String?

The title for the search results view.

var displaysSearchBarInNavigationBar: Bool

Specifies that the navigation bar contains a search bar.

var navigationItem: UINavigationItem?

Represents the search display controller in a navigation controller’s navigation bar.

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

### Deprecated classes

class UIActionSheet

A view that presents a set of alternatives for how to proceed with a task.

Deprecated

class UIAlertView

A view that displays an alert message.

Deprecated

class UIDocumentMenuViewController

A list of all the available document providers for a given file type and mode, in addition to custom menu items that you add.

Deprecated

class UILocalNotification

A notification that an app can schedule for presentation at a specific date and time.

Deprecated

class UIMenuController

The menu interface for the Cut, Copy, Paste, Select, Select All, and Delete commands.

Deprecated

class UIMenuItem

A custom item in the editing menu managed by the menu controller.

Deprecated

class UIMutableUserNotificationAction

A modifiable version of the user notification action class.

Deprecated

class UIMutableUserNotificationCategory

Information about custom actions that your app can perform in response to a local or push notification.

Deprecated

class UIPopoverController

An object that manages the presentation of content in a popover.

Deprecated

class UIPreviewAction

A preview action, or *peek quick action*, that displays below a peek when a user swipes the peek upward.

Deprecated

class UIPreviewActionGroup

A group of one or more child quick actions, each an instance of the preview action class.

Deprecated

class UIStoryboardPopoverSegue

A specific type of segue for presenting content in a popover.

Deprecated

class UIUserNotificationAction

A custom action that your app can perform in response to a remote or local notification.

Deprecated

class UIUserNotificationCategory

Information about custom actions that your app can perform in response to a local or push notification.

Deprecated

class UIUserNotificationSettings

The types of notifications that can be displayed to the user by your app.

Deprecated

