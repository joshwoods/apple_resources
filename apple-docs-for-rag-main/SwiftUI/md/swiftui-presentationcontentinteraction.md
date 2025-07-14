

- SwiftUI
-  PresentationContentInteraction 

Structure

# PresentationContentInteraction

A behavior that you can use to influence how a presentation responds to swipe gestures.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
struct PresentationContentInteraction
```

## Overview

Use values of this type with the presentationContentInteraction(_:) modifier.

## Topics

### Getting interaction behaviors

static var automatic: PresentationContentInteraction

The default swipe behavior for the presentation.

static var resizes: PresentationContentInteraction

A behavior that prioritizes resizing a presentation when swiping, rather than scrolling the content of the presentation.

static var scrolls: PresentationContentInteraction

A behavior that prioritizes scrolling the content of a presentation when swiping, rather than resizing the presentation.

## Relationships

### Conforms To

- Equatable
- Sendable

## See Also

### Configuring a sheet’s height

func presentationDetents(Set&lt;PresentationDetent>) -> some View

Sets the available detents for the enclosing sheet.

func presentationDetents(Set&lt;PresentationDetent>, selection: Binding&lt;PresentationDetent>) -> some View

Sets the available detents for the enclosing sheet, giving you programmatic control of the currently selected detent.

func presentationContentInteraction(PresentationContentInteraction) -> some View

Configures the behavior of swipe gestures on a presentation.

func presentationDragIndicator(Visibility) -> some View

Sets the visibility of the drag indicator on top of a sheet.

struct PresentationDetent

A type that represents a height where a sheet naturally rests.

protocol CustomPresentationDetent

The definition of a custom detent with a calculated height.

