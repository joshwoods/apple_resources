

- SwiftUI
-  Prominence 

Enumeration

# Prominence

A type indicating the prominence of a view hierarchy.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
enum Prominence
```

## Topics

### Getting prominence options

case standard

The standard prominence.

case increased

An increased prominence.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Configuring headers

func headerProminence(Prominence) -> some View

Sets the header prominence for this view.

var headerProminence: Prominence

The prominence to apply to section headers within a view.

var defaultMinListHeaderHeight: CGFloat?

The default minimum height of a header in a list.

