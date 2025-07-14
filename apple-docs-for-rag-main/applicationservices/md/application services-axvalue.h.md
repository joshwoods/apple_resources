

- Application Services
-  AXValue.h 

API Collection

# AXValue.h

This header contains functions and data types for working with AXValueType wrappers.

## Overview

See the Overview section above for header-level documentation.

### Overview

#### Included Headers

- \

- \

- \

## Topics

### Miscellaneous

func AXValueCreate(AXValueType, UnsafeRawPointer) -> AXValue?

func AXValueGetType(AXValue) -> AXValueType

func AXValueGetTypeID() -> CFTypeID

func AXValueGetValue(AXValue, AXValueType, UnsafeMutableRawPointer) -> Bool

### Data Types

See the Overview section above for header-level documentation.

class AXValue

enum AXValueType

