

- Application Services
-  UniversalAccess.h 

API Collection

# UniversalAccess.h

This header file contains functions that give applications the ability to control the zoom focus. Using these functions, an application can tell the macOS Universal Access zoom feature what part of its user interface needs focus.

## Overview

See the Overview section above for header-level documentation.

### Overview

#### Included Headers

- \

- \

## Topics

### Miscellaneous

func UAZoomChangeFocus(UnsafePointer&lt;CGRect>!, UnsafePointer&lt;CGRect>!, UAZoomChangeFocusType) -> OSStatus

Tells the Universal Access zoom feature where it should focus.

func UAZoomEnabled() -> Bool

Determines if the Universal Access zoom feature is enabled.

### Data Types

See the Overview section above for header-level documentation.

typealias UAZoomChangeFocusType

Defines the Universal Access zoom change focus type.

### Constants

See the Overview section above for header-level documentation.

UAZoomFocusTypes

Values that tell the Universal Access zoom feature what type of event is causing the change in zoom focus.

