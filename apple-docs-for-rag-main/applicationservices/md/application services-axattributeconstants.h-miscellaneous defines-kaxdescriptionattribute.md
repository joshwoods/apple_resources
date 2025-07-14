

- Application Services
- AXAttributeConstants.h
- Miscellaneous Defines
-  kAXDescriptionAttribute 

Global Variable

# kAXDescriptionAttribute

macOS 10.4+

``` source
var kAXDescriptionAttribute: String { get }
```

## Discussion

The purpose of this accessibility object. The description string must be localizable and human-intelligible and it must be all lower case and include no punctuation. The string should briefly describe this accessibility object’s purpose, without including the object’s role description. This attribute is required for all accessibility objects that do not provide enough descriptive information in the title attribute.

