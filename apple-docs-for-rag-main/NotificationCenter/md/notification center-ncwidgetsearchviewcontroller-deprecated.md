

- Notification Center
-  NCWidgetSearchViewController Deprecated

Class

# NCWidgetSearchViewController

An object that provides a default search view within a macOS Today widget.

macOS 10.10–11.0Deprecated

``` source
@MainActor
class NCWidgetSearchViewController
```

Deprecated

Use WidgetKit instead.

## Overview

The `NCWidgetSearchViewController` class provides a default search view within a Today widget. A search view controller works together with its delegate to perform searches on the user’s input and display results from which a user can choose. To learn about the search view controller delegate methods, see NCWidgetSearchViewDelegate.

When a widget is in editing mode, it can enable search for new content by instantiating an `NCWidgetSearchViewController` object and presenting it using present(inWidget:). The search view controller displays the default search field and a list of results. It uses its delegate to perform the search itself.

## Topics

### Enabling Search

var delegate: (any NCWidgetSearchViewDelegate)?

The search view controller’s delegate or `nil` if the receiver doesn’t have a delegate.

protocol NCWidgetSearchViewDelegate

The interface for enabling user searches in the search view controller of a macOS Today widget.

### Displaying the Search Interface

var searchDescription: String?

A localized description of the nature of the search.

var searchResultsPlaceholderString: String?

A localized phrase displayed in the results list when no search results are available.

### Displaying Search Results

var searchResultKeyPath: String?

A key path for the string property to display for each object in the search results array.

var searchResults: [Any]?

An array of search results.

## Relationships

### Inherits From

- NSViewController

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSEditor
- NSExtensionRequestHandling
- NSObjectProtocol
- NSSeguePerforming
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceItemIdentification
- Sendable

## See Also

### Search View

protocol NCWidgetSearchViewDelegate

The interface for enabling user searches in the search view controller of a macOS Today widget.

Deprecated

