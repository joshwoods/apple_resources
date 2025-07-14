

- SwiftUI
-  PresentationAdaptation 

Structure

# PresentationAdaptation

Strategies for adapting a presentation to a different size class.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
struct PresentationAdaptation
```

## Overview

Use values of this type with the presentationCompactAdaptation(_:) and presentationCompactAdaptation(horizontal:vertical:) modifiers.

## Topics

### Getting adaptation strategies

static var automatic: PresentationAdaptation

Use the default presentation adaptation.

static var none: PresentationAdaptation

Don’t adapt for the size class, if possible.

static var fullScreenCover: PresentationAdaptation

Prefer a full-screen-cover appearance when adapting for size classes.

static var popover: PresentationAdaptation

Prefer a popover appearance when adapting for size classes.

static var sheet: PresentationAdaptation

Prefer a sheet appearance when adapting for size classes.

## Relationships

### Conforms To

- Sendable

## See Also

### Adapting a presentation size

func presentationCompactAdaptation(horizontal: PresentationAdaptation, vertical: PresentationAdaptation) -> some View

Specifies how to adapt a presentation to horizontally and vertically compact size classes.

func presentationCompactAdaptation(PresentationAdaptation) -> some View

Specifies how to adapt a presentation to compact size classes.

func presentationSizing(some PresentationSizing) -> some View

Sets the sizing of the containing presentation.

protocol PresentationSizing

A type that defines the size of the presentation content and how the presentation size adjusts to its content’s size changing.

struct PresentationSizingRoot

A proxy to a view provided to the presentation with a defined presentation size.

struct PresentationSizingContext

Contextual information about a presentation.

