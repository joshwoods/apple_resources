

- Application Services
-  AXTextAttributedString.h 

API Collection

# AXTextAttributedString.h

This header file contains definitions of constants used with accessibility objects that represent attributed strings. An attributed string is an association of a range of characters and their attributes, such as color and font. If an accessibility object represents an attributed string, the value of its `kAXParameterizedAttributeStringAttribute` attribute is an attributed string object (a `CFAttributedStringRef` or an `NSAttributedString`) that uses the constants defined in this header file to define its attributes.

## Overview

### Included Headers

- \

## Topics

### Constants

See the Overview section above for header-level documentation.

Global Variables

enum AXUnderlineStyle

Values that describe the style of underlining (used with the kAXUnderlineTextAttribute attribute).

