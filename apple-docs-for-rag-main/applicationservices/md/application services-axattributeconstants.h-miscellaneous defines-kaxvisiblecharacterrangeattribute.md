

- Application Services
- AXAttributeConstants.h
- Miscellaneous Defines
-  kAXVisibleCharacterRangeAttribute 

Global Variable

# kAXVisibleCharacterRangeAttribute

macOS 10.3+

``` source
var kAXVisibleCharacterRangeAttribute: String { get }
```

## Discussion

Indicates the range of characters (not bytes) that are scrolled into view within this accessibility object. This attribute is required only for accessibility objects that represent an editable text area (objects of role `AXTextArea`), not for any other text-related accessibility objects.

