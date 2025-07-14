

- UIKit
-  UISearchDisplayDelegate Deprecated

Protocol

# UISearchDisplayDelegate

The interface for the delegate of a search display controller.

iOSiPadOSMac Catalyst

``` source
@MainActor
protocol UISearchDisplayDelegate : NSObjectProtocol
```

Deprecated

Use UISearchControllerDelegate instead.

## Overview

This protocol defines delegate methods for UISearchDisplayController objects.

## Topics

### Responding to search state change

func searchDisplayControllerWillBeginSearch(UISearchDisplayController)

Tells the delegate that the controller is about to begin searching.

func searchDisplayControllerDidBeginSearch(UISearchDisplayController)

Tells the delegate that the controller has started searching.

func searchDisplayControllerWillEndSearch(UISearchDisplayController)

Tells the delegate that the controller is about to end searching.

func searchDisplayControllerDidEndSearch(UISearchDisplayController)

Tells the delegate that the controller has finished searching.

### Loading and unloading the table view

func searchDisplayController(UISearchDisplayController, didLoadSearchResultsTableView: UITableView)

Tells the delegate that the controller has loaded its table view.

func searchDisplayController(UISearchDisplayController, willUnloadSearchResultsTableView: UITableView)

Tells the delegate that the controller is about to unload its table view.

### Showing and hiding the table view

func searchDisplayController(UISearchDisplayController, willShowSearchResultsTableView: UITableView)

Tells the delegate that the controller is about to display its table view.

func searchDisplayController(UISearchDisplayController, didShowSearchResultsTableView: UITableView)

Tells the delegate that the controller just displayed its table view.

func searchDisplayController(UISearchDisplayController, willHideSearchResultsTableView: UITableView)

Tells the delegate that the controller is about to hide its table view.

func searchDisplayController(UISearchDisplayController, didHideSearchResultsTableView: UITableView)

Tells the delegate that the controller just hid its table view.

### Responding to changes in search criteria

func searchDisplayController(UISearchDisplayController, shouldReloadTableForSearch: String?) -> Bool

Asks the delegate if the table view should be reloaded for a given search string.

func searchDisplayController(UISearchDisplayController, shouldReloadTableForSearchScope: Int) -> Bool

Asks the delegate if the table view should be reloaded for a given scope.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Deprecated protocols

protocol UIAccelerometerDelegate

The interface for receiving acceleration-related data from the system.

Deprecated

protocol UIActionSheetDelegate

The interface for the delegate of an action sheet object.

Deprecated

protocol UIAlertViewDelegate

The interface for the delegate of an alert view object.

Deprecated

protocol UIPopoverControllerDelegate

The interface for the delegate of a popover controller object.

Deprecated

protocol UIViewControllerPreviewing

A set of methods that define the interface for configuring a previewing view controller on devices that support 3D Touch.

Deprecated

protocol UIViewControllerPreviewingDelegate

A set of methods used by the delegate to respond, with a preview view controller and a commit view controller, to the user pressing a view object on the screen of a device that supports 3D Touch.

Deprecated

