

- SwiftUI
-  ControlSize 

Enumeration

# ControlSize

The size classes, like regular or small, that you can apply to controls within a view.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.15+visionOS 1.0+watchOS 9.0+

``` source
enum ControlSize
```

## Topics

### Getting control sizes

case mini

A control version that is minimally sized.

case small

A control version that is proportionally smaller size for space-constrained views.

case regular

A control version that is the default size.

case large

A control version that is prominently sized.

case extraLarge

A control version that is substantially sized. The largest control size. Resolves to ControlSize.large on platforms other than visionOS.

## Relationships

### Conforms To

- CaseIterable
- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Sizing controls

func controlSize(ControlSize) -> some View

Sets the size for controls within this view.

var controlSize: ControlSize

The size to apply to controls within a view.

