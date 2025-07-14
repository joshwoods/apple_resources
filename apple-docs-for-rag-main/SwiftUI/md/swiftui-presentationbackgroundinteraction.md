

- SwiftUI
-  PresentationBackgroundInteraction 

Structure

# PresentationBackgroundInteraction

The kinds of interaction available to views behind a presentation.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
struct PresentationBackgroundInteraction
```

## Overview

Use values of this type with the presentationBackgroundInteraction(_:) modifier.

## Topics

### Getting interaction types

static var automatic: PresentationBackgroundInteraction

The default background interaction for the presentation.

static var disabled: PresentationBackgroundInteraction

People can’t interact with the view behind a presentation.

static var enabled: PresentationBackgroundInteraction

People can interact with the view behind a presentation.

static func enabled(upThrough: PresentationDetent) -> PresentationBackgroundInteraction

People can interact with the view behind a presentation up through a specified detent.

## Relationships

### Conforms To

- Sendable

## See Also

### Styling a sheet and its background

func presentationCornerRadius(CGFloat?) -> some View

Requests that the presentation have a specific corner radius.

func presentationBackground&lt;S>(S) -> some View

Sets the presentation background of the enclosing sheet using a shape style.

func presentationBackground&lt;V>(alignment: Alignment, content: () -> V) -> some View

Sets the presentation background of the enclosing sheet to a custom view.

func presentationBackgroundInteraction(PresentationBackgroundInteraction) -> some View

Controls whether people can interact with the view behind a presentation.

