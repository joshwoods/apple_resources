

- UIKit
- UITableView
-  UITableView.SelfSizingInvalidation 

Enumeration

# UITableView.SelfSizingInvalidation

Constants that describe modes for invalidating the size of self-sizing table view cells.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 16.0+visionOS 1.0+

``` source
enum SelfSizingInvalidation
```

## Overview

Use these constants with the selfSizingInvalidation property.

## Topics

### Constants

case disabled

A mode that disables self-sizing invalidation.

case enabled

A mode that enables manual self-sizing invalidation.

case enabledIncludingConstraints

A mode that enables automatic self-sizing invalidation after Auto Layout changes.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Resizing self-sizing cells

var selfSizingInvalidation: UITableView.SelfSizingInvalidation

The mode that the table view uses for invalidating the size of self-sizing cells.

