

- Application Services
- AXValue.h
-  AXValueType 

Enumeration

# AXValueType

macOS 10.2+

``` source
enum AXValueType : UInt32, @unchecked Sendable
```

## Overview

These are AXValueType wrappers for other structures. You must use the AXValueCreate and AXValueGetValue functions to convert between the wrapped structure and the native structure.

## Topics

### Constants

kAXValueCGPointType

kAXValueCGSizeType

kAXValueCGRectType

kAXValueCFRangeType

kAXValueAXErrorType

kAXValueIllegalType

### Enumeration Cases

case axError

case cfRange

case cgPoint

case cgRect

case cgSize

case illegal

## Relationships

### Conforms To

- Sendable

