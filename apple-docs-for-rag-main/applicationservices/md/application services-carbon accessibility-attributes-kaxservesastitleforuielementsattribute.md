

- Application Services
- Carbon Accessibility
- Attributes
-  kAXServesAsTitleForUIElementsAttribute 

Global Variable

# kAXServesAsTitleForUIElementsAttribute

macOS 10.4+

``` source
var kAXServesAsTitleForUIElementsAttribute: String { get }
```

## Discussion

An array of accessibility objects for which this accessibility object serves as the title. For example, a piece of static text can serve as a title for one or more user interface elements. Because this static text string is not displayed as part of any user interface element’s visual interface, an assistive application does not know the title is associated with user interface elements. By including this attribute in the accessibility object representing the title, you specify the accessibility objects with which this title is associated.

