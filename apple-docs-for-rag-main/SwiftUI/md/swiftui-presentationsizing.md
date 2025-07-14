

- SwiftUI
-  PresentationSizing 

Protocol

# PresentationSizing

A type that defines the size of the presentation content and how the presentation size adjusts to its content’s size changing.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
protocol PresentationSizing
```

## Overview

You don’t need to define your own version of this protocol. The system implementations of form, page, and fitted are conveniences that automatically adapt to different device and screen sizes. If you do want to define your own sizing, first consider using the modifiers `PresenationSizing/sticky(horizontal:vertical:)` and fitted(horizontal:vertical:). For example, to define your own sizing that proposes a 400x400 square size:

```
protocol SquareSizing: PresentationSizing {
    func proposedSize(
        for subview: PresentationSizingRoot,
        context: PresentationSizingContext
    ) {
        .init(width: 400, height: 400)
    }
}

extension PresentationSizing where Self == SquareSizing {
    public static var square: Self { SquareSizing() }
}
```

Then, at the callsite, you can modify `.square` just like system sizings, for example, to fit its content vertically:

```
.presentationSizing(.square.fitted(horizontal: false, vertical: true))
```

See Also

presentationSizing(_:)

## Topics

### Getting built-in presentation size

static var automatic: AutomaticPresentationSizing

The default presentation sizing, appropriate for the platform.

static var fitted: FittedPresentationSizing

The presentation sizing is dictated by the ideal size of the content

static var form: FormPresentationSizing

The size is appropriate for forms and slightly less wide than`.page`

static var page: PagePresentationSizing

The size is roughly the size of a page of paper, appropriate for informational or compositional content.

### Creating custom presentation size

func fitted(horizontal: Bool, vertical: Bool) -> some PresentationSizing

func proposedSize(for: PresentationSizingRoot, context: PresentationSizingContext) -> ProposedViewSize

**Required**

func sticky(horizontal: Bool, vertical: Bool) -> some PresentationSizing

Modifies self to be sticky in the specified dimensions — growing, but not shrinking.

### Supporting types

struct AutomaticPresentationSizing

The default presentation sizing, appropriate for the platform.

struct FittedPresentationSizing

The size of the presentation is dictated by the ideal size of the content.

struct FormPresentationSizing

The size is appropriate for forms and slightly less wide than`.page`

struct PagePresentationSizing

The size is roughly the size of a page of paper, appropriate for informational or compositional content.

## Relationships

### Conforming Types

- AutomaticPresentationSizing
- FittedPresentationSizing
- FormPresentationSizing
- PagePresentationSizing

## See Also

### Adapting a presentation size

func presentationCompactAdaptation(horizontal: PresentationAdaptation, vertical: PresentationAdaptation) -> some View

Specifies how to adapt a presentation to horizontally and vertically compact size classes.

func presentationCompactAdaptation(PresentationAdaptation) -> some View

Specifies how to adapt a presentation to compact size classes.

struct PresentationAdaptation

Strategies for adapting a presentation to a different size class.

func presentationSizing(some PresentationSizing) -> some View

Sets the sizing of the containing presentation.

struct PresentationSizingRoot

A proxy to a view provided to the presentation with a defined presentation size.

struct PresentationSizingContext

Contextual information about a presentation.

