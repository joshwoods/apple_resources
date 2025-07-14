

- UIKit
-  UISearchBarDelegate 

Protocol

# UISearchBarDelegate

A collection of optional methods that you implement to make a search bar control functional.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
protocol UISearchBarDelegate : UIBarPositioningDelegate
```

## Overview

A UISearchBar object provides the user interface for a search field on a bar, but it’s the application’s responsibility to implement the actions when buttons are tapped. At a minimum, the delegate needs to perform the actual search when text is entered in the text field.

## Topics

### Managing the search text

func searchBar(UISearchBar, textDidChange: String)

Tells the delegate that the user changed the search text.

func searchBar(UISearchBar, shouldChangeTextIn: NSRange, replacementText: String) -> Bool

Ask the delegate if text in a specified range should be replaced with given text.

func searchBarShouldBeginEditing(UISearchBar) -> Bool

Asks the delegate if editing should begin in the specified search bar.

func searchBarTextDidBeginEditing(UISearchBar)

Tells the delegate when the user begins editing the search text.

func searchBarShouldEndEditing(UISearchBar) -> Bool

Asks the delegate if editing should stop in the specified search bar.

func searchBarTextDidEndEditing(UISearchBar)

Tells the delegate that the user finished editing the search text.

### Responding to clicks in search controls

func searchBarBookmarkButtonClicked(UISearchBar)

Tells the delegate that the bookmark button was tapped.

func searchBarCancelButtonClicked(UISearchBar)

Tells the delegate that the cancel button was tapped.

func searchBarSearchButtonClicked(UISearchBar)

Tells the delegate that the search button was tapped.

func searchBarResultsListButtonClicked(UISearchBar)

Tells the delegate that the search results list button was tapped.

### Responding to scope button changes

func searchBar(UISearchBar, selectedScopeButtonIndexDidChange: Int)

Tells the delegate that the scope button selection changed.

## Relationships

### Inherits From

- NSObjectProtocol
- UIBarPositioningDelegate

## See Also

### Handling search bar interactions

var delegate: (any UISearchBarDelegate)?

The search bar’s delegate object.

