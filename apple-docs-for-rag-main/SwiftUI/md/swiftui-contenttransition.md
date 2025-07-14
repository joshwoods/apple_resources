

- SwiftUI
-  ContentTransition 

Structure

# ContentTransition

A kind of transition that applies to the content within a single view, rather than to the insertion or removal of a view.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct ContentTransition
```

## Overview

Set the behavior of content transitions within a view with the contentTransition(_:) modifier, passing in one of the defined transitions, such as opacity or interpolate as the parameter.

Tip

Content transitions only take effect within transactions that apply an Animation to the views inside the contentTransition(_:) modifier.

Content transitions only take effect within the context of an Animation block.

## Topics

### Getting content transitions

static let identity: ContentTransition

The identity content transition, which indicates that content changes shouldn’t animate.

static let interpolate: ContentTransition

A content transition that indicates the views attempt to interpolate their contents during transitions, where appropriate.

static func numericText(countsDown: Bool) -> ContentTransition

Creates a content transition intended to be used with `Text` views displaying numeric text. In certain environments changes to the text will enable a nonstandard transition tailored to numeric characters that count up or down.

static func numericText(value: Double) -> ContentTransition

Creates a content transition intended to be used with `Text` views displaying numbers.

static let opacity: ContentTransition

A content transition that indicates content fades from transparent to opaque on insertion, and from opaque to transparent on removal.

static var symbolEffect: ContentTransition

A content transition that applies the default symbol effect transition to symbol images within the inserted or removed view hierarchy. Other views are unaffected by this transition.

static func symbolEffect&lt;T>(T, options: SymbolEffectOptions) -> ContentTransition

Creates a content transition that applies the symbol Replace animation to symbol images that it is applied to.

## Relationships

### Conforms To

- Equatable
- Sendable

## See Also

### Defining transitions

func transition(_:)

Associates a transition with the view.

protocol Transition

A description of view changes to apply when a view is added to and removed from the view hierarchy.

struct TransitionProperties

The properties a `Transition` can have.

enum TransitionPhase

An indication of which the current stage of a transition.

struct AsymmetricTransition

A composite `Transition` that uses a different transition for insertion versus removal.

struct AnyTransition

A type-erased transition.

func contentTransition(ContentTransition) -> some View

Modifies the view to use a given transition as its method of animating changes to the contents of its views.

var contentTransition: ContentTransition

The current method of animating the contents of views.

var contentTransitionAddsDrawingGroup: Bool

A Boolean value that controls whether views that render content transitions use GPU-accelerated rendering.

struct PlaceholderContentView

A placeholder used to construct an inline modifier, transition, or other helper type.

func navigationTransition(some NavigationTransition) -> some View

Sets the navigation transition style for this view.

protocol NavigationTransition

A type that defines the transition to use when navigating to a view.

func matchedTransitionSource(id: some Hashable, in: Namespace.ID) -> some View

Identifies this view as the source of a navigation transition, such as a zoom transition.

func matchedTransitionSource(id: some Hashable, in: Namespace.ID, configuration: (EmptyMatchedTransitionSourceConfiguration) -> some MatchedTransitionSourceConfiguration) -> some View

Identifies this view as the source of a navigation transition, such as a zoom transition.

protocol MatchedTransitionSourceConfiguration

A configuration that defines the appearance of a matched transition source.

