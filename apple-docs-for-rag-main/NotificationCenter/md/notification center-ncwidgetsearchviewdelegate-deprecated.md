

- Notification Center
-  NCWidgetSearchViewDelegate Deprecated

Protocol

# NCWidgetSearchViewDelegate

The interface for enabling user searches in the search view controller of a macOS Today widget.

macOS 10.10–11.0Deprecated

``` source
protocol NCWidgetSearchViewDelegate : NSObjectProtocol
```

Deprecated

Use WidgetKit instead.

## Overview

The `NCWidgetSearchViewDelegate` protocol defines methods that enable user searches in the search view controller of a Today widget. The delegate of an NCWidgetSearchViewController must adopt the NCWidgetSearchViewDelegate protocol.

The search view controller tells its delegate to perform a search on a user’s input and the delegate returns the results by setting the controller’s searchResults property. The search view controller also tells its delegate when a user clears the search field or chooses a search result, so that the delegate can prepare for a new search or dismissal.

## Topics

### Searching Your Content

func widgetSearch(NCWidgetSearchViewController, searchForTerm: String, maxResults: Int)

Asks the delegate to search using the specified term.

**Required**

### Responding to User Choices

func widgetSearch(NCWidgetSearchViewController, resultSelected: Any)

Tells the delegate that a user chose the specified search result.

**Required**

func widgetSearchTermCleared(NCWidgetSearchViewController)

Tells the delegate that a user cleared the search field.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Search View

class NCWidgetSearchViewController

An object that provides a default search view within a macOS Today widget.

Deprecated

