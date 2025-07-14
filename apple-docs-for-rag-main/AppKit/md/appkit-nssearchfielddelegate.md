

- AppKit
-  NSSearchFieldDelegate 

Protocol

# NSSearchFieldDelegate

A protocol that a search field delegate can use to determine when a search started or ended.

macOS

``` source
protocol NSSearchFieldDelegate : NSTextFieldDelegate
```

## Topics

### Detecting the Start and End of a Search

func searchFieldDidStartSearching(NSSearchField)

The method that is called when the search field begins searching for content.

func searchFieldDidEndSearching(NSSearchField)

The method that is called when the search field has ended its search for content.

## Relationships

### Inherits From

- NSControlTextEditingDelegate
- NSObjectProtocol
- NSTextFieldDelegate

## See Also

### Managing Search

var delegate: (any NSSearchFieldDelegate)?

The delegate for the search field, or `nil` if the search field doesn’t have a delegate.

