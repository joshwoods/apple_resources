

- SwiftUI
-  Visibility 

Enumeration

# Visibility

The visibility of a UI element, chosen automatically based on the platform, current context, and other factors.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@frozen
enum Visibility
```

## Overview

For example, the preferred visibility of list row separators can be configured using the listRowSeparator(_:edges:).

## Topics

### Getting visibility options

case automatic

The element may be visible or hidden depending on the policies of the component accepting the visibility configuration.

case visible

The element may be visible.

case hidden

The element may be hidden.

## Relationships

### Conforms To

- BitwiseCopyable
- CaseIterable
- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Hiding system elements

func labelsHidden() -> some View

Hides the labels of any controls contained within this view.

func labelsVisibility(Visibility) -> some View

Controls the visibility of labels of any controls contained within this view.

var labelsVisibility: Visibility

The labels visibility set by labelsVisibility(_:).

func menuIndicator(Visibility) -> some View

Sets the menu indicator visibility for controls within this view.

func statusBarHidden(Bool) -> some View

Sets the visibility of the status bar.

func persistentSystemOverlays(Visibility) -> some View

Sets the preferred visibility of the non-transient system views overlaying the app.

