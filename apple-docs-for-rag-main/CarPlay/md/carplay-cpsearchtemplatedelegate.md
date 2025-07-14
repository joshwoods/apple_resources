

- CarPlay
-  CPSearchTemplateDelegate 

Protocol

# CPSearchTemplateDelegate

The interface for an object that serves as the search template’s delegate.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
protocol CPSearchTemplateDelegate : NSObjectProtocol
```

## Topics

### Updating Search Text

func searchTemplate(CPSearchTemplate, updatedSearchText: String, completionHandler: ([CPListItem]) -> Void)

Tells the delegate that the user updated the search criteria text.

**Required**

### Selecting a Search Result Item

func searchTemplate(CPSearchTemplate, selectedResult: CPListItem, completionHandler: () -> Void)

Tells the delegate that the user selected an item from the search result.

**Required**

### Pressing the Search Button

func searchTemplateSearchButtonPressed(CPSearchTemplate)

Tells the delegate that the user tapped the keyboard’s search button.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Providing a Search Template Delegate

var delegate: (any CPSearchTemplateDelegate)?

The object that serves as the search template’s delegate.

