

- Application Services
- Carbon Accessibility
- Attributes
-  kAXLinkedUIElementsAttribute 

Global Variable

# kAXLinkedUIElementsAttribute

macOS 10.4+

``` source
var kAXLinkedUIElementsAttribute: String { get }
```

## Discussion

An array of accessibility objects with which this accessibility object is related. For example, the contents of a list item can be displayed in another pane or window. The list item and the separately displayed contents are related, but this relationship may not be apparent to an assistive application. To make such a relationship explicit, you include this attribute in the accessibility objects representing the related user interface elements.

