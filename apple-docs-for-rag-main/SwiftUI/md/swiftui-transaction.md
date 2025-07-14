

- SwiftUI
-  Transaction 

Structure

# Transaction

The context of the current state-processing update.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@frozen
struct Transaction
```

## Overview

Use a transaction to pass an animation between views in a view hierarchy.

The root transaction for a state change comes from the binding that changed, plus any global values set by calling withTransaction(_:_:) or withAnimation(_:_:).

## Topics

### Creating a transaction

init()

Creates a transaction.

init(animation: Animation?)

Creates a transaction and assigns its animation property.

### Managing animations

var animation: Animation?

The animation, if any, associated with the current state change.

var disablesAnimations: Bool

A Boolean value that indicates whether views should disable animations.

func addAnimationCompletion(criteria: AnimationCompletionCriteria, () -> Void)

Adds a completion to run when the animations created with this transaction are all complete.

### Managing window dismissal

var dismissBehavior: DismissBehavior

The behavior for how windows will dismiss programmatically when used in conjunction with DismissWindowAction.

### Getting information about a transaction

var isContinuous: Bool

A Boolean value that indicates whether the transaction originated from an action that produces a sequence of values.

var scrollTargetAnchor: UnitPoint?

The preferred alignment of the view within a scroll view’s visible region when scrolling to a view.

var tracksVelocity: Bool

Whether this transaction will track the velocity of any animatable properties that change.

subscript&lt;K>(K.Type) -> K.Value

Accesses the transaction value associated with a custom key.

### Instance Properties

var scrollContentOffsetAdjustmentBehavior: ScrollContentOffsetAdjustmentBehavior

The behavior a scroll view will have regarding content offset adjustments for the current transaction.

var scrollPositionUpdatePreservesVelocity: Bool

Whether a programmatic update to the scroll position of a scroll view preserves the current velocity of any active scroll of the scroll view.

## See Also

### Moving an animation to another view

func withTransaction&lt;Result>(Transaction, () throws -> Result) rethrows -> Result

Executes a closure with the specified transaction and returns the result.

func withTransaction&lt;R, V>(WritableKeyPath&lt;Transaction, V>, V, () throws -> R) rethrows -> R

Executes a closure with the specified transaction key path and value and returns the result.

func transaction((inout Transaction) -> Void) -> some View

Applies the given transaction mutation function to all animations used within the view.

func transaction(value: some Equatable, (inout Transaction) -> Void) -> some View

Applies the given transaction mutation function to all animations used within the view.

func transaction&lt;V>((inout Transaction) -> Void, body: (PlaceholderContentView&lt;Self>) -> V) -> some View

Applies the given transaction mutation function to all animations used within the `body` closure.

macro Entry()

Creates an environment values, transaction, container values, or focused values entry.

protocol TransactionKey

A key for accessing values in a transaction.

