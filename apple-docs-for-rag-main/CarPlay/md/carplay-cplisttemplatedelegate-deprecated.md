

- CarPlay
-  CPListTemplateDelegate Deprecated

Protocol

# CPListTemplateDelegate

The interface an object implements to serve as the delegate for a list template.

iOS 12.0–14.0DeprecatediPadOS 12.0–14.0DeprecatedMac Catalyst 13.1–14.0Deprecated

``` source
protocol CPListTemplateDelegate : NSObjectProtocol
```

## Topics

### Getting the Selected Item

func listTemplate(CPListTemplate, didSelect: CPListItem, completionHandler: () -> Void)

Tells the delegate when the user selects a list item.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Responding to List Events

var delegate: (any CPListTemplateDelegate)?

The object that serves as the delegate to the list template.

Deprecated

