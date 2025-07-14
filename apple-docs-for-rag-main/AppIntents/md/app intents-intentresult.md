

- App Intents
-  IntentResult 

Protocol

# IntentResult

A type that contains the result of performing an action, and includes optional information to deliver back to the initiator.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol IntentResult : Sendable
```

## Overview

Instead of implementing this protocol, use the ReturnsValue, OpensAppIntent, ProvidesDialog, and ShowsSnippetView type aliases on your perform() implementation in combination with the result() methods as shown in the following example:

```
func perform() async throws -> some ReturnsValue & OpensAppIntent {
    .result(value: 1, opensIntent: MyOpensIntent())
}
```

## Topics

### Getting the result value

var value: Self.Value?

**Required**

### Communicating the result to the user

associatedtype Dialog = Never

**Required**

### Associated Types

associatedtype OpensAppIntent : AppIntent = Never

**Required**

associatedtype Snippet = Never

**Required**

associatedtype Value : _IntentValue = Never

**Required**

### Type Methods

static func result() -> Self

Indicates the `AppIntent` finished performing

static func result&lt;Intent>(actionButtonIntent: Intent) -> Self

Indicates the Intent finished performing with an `AppIntent` to continue with

static func result&lt;Intent>(actionButtonIntent: Intent, activityIdentifier: String) -> Self

Indicates the Intent finished performing with an `AppIntent` to continue with

static func result&lt;Intent>(actionButtonIntent: Intent, activityIdentifier: String, dialog: IntentDialog) -> Self

Indicates the Intent finished performing with an `AppIntent` to continue with

static func result&lt;Intent>(actionButtonIntent: Intent, dialog: IntentDialog) -> Self

Indicates the Intent finished performing with an `AppIntent` to continue with

static func result&lt;Content>(content: () -> Content) -> Self

Indicates the `AppIntent` finished performing

static func result(dialog: IntentDialog) -> Self

Indicates the `AppIntent` finished performing

static func result&lt;Content>(dialog: IntentDialog, content: () -> Content) -> Self

Indicates the `AppIntent` finished performing

static func result&lt;Content>(dialog: IntentDialog, view: Content) -> Self

Indicates the `AppIntent` finished performing

static func result(opensIntent: some AppIntent) -> Self

Indicates the `AppIntent` finished performing

static func result&lt;OpensAppIntent, Content>(opensIntent: OpensAppIntent, content: () -> Content) -> Self

static func result&lt;Content>(opensIntent: some AppIntent, content: () -> Content) -> Self

Indicates the `AppIntent` finished performing

static func result(opensIntent: some AppIntent, dialog: IntentDialog) -> Self

Indicates the `AppIntent` finished performing

static func result&lt;OpensAppIntent, Content>(opensIntent: OpensAppIntent, dialog: IntentDialog, content: () -> Content) -> Self

static func result&lt;Content>(opensIntent: some AppIntent, dialog: IntentDialog, content: () -> Content) -> Self

Indicates the `AppIntent` finished performing

static func result&lt;Content>(opensIntent: some AppIntent, dialog: IntentDialog, view: Content) -> Self

Indicates the `AppIntent` finished performing

static func result&lt;OpensAppIntent, Content>(opensIntent: OpensAppIntent, dialog: IntentDialog, view: Content) -> Self

static func result&lt;OpensAppIntent, Content>(opensIntent: OpensAppIntent, view: Content) -> Self

static func result&lt;Content>(opensIntent: some AppIntent, view: Content) -> Self

Indicates the `AppIntent` finished performing

static func result&lt;Value>(value: Value) -> Self

Indicates the `AppIntent` finished performing

static func result&lt;Value, Intent>(value: Value, actionButtonIntent: Intent) -> Self

Indicates the Intent finished performing with an `AppIntent` to continue with

static func result&lt;Value, Intent>(value: Value, actionButtonIntent: Intent, activityIdentifier: String) -> Self

Indicates the Intent finished performing with an `AppIntent` to continue with

static func result&lt;Value, Intent>(value: Value, actionButtonIntent: Intent, activityIdentifier: String, dialog: IntentDialog) -> Self

Indicates the Intent finished performing with an `AppIntent` to continue with

static func result&lt;Value, Intent>(value: Value, actionButtonIntent: Intent, dialog: IntentDialog) -> Self

Indicates the Intent finished performing with an `AppIntent` to continue with

static func result&lt;Value, Content>(value: Value, content: () -> Content) -> Self

Indicates the `AppIntent` finished performing

static func result&lt;Value>(value: Value, dialog: IntentDialog) -> Self

Indicates the `AppIntent` finished performing

static func result&lt;Value, Content>(value: Value, dialog: IntentDialog, content: () -> Content) -> Self

Indicates the `AppIntent` finished performing

static func result&lt;Value, Content>(value: Value, dialog: IntentDialog, view: Content) -> Self

Indicates the `AppIntent` finished performing

static func result&lt;Value>(value: Value, opensIntent: some AppIntent) -> Self

Indicates the `AppIntent` finished performing

static func result&lt;Value, Content>(value: Value, opensIntent: some AppIntent, content: () -> Content) -> Self

Indicates the `AppIntent` finished performing

static func result&lt;Value, OpensAppIntent, Content>(value: Value, opensIntent: OpensAppIntent, content: () -> Content) -> Self

static func result&lt;Value>(value: Value, opensIntent: some AppIntent, dialog: IntentDialog) -> Self

Indicates the `AppIntent` finished performing

static func result&lt;Value, OpensAppIntent, Content>(value: Value, opensIntent: OpensAppIntent, dialog: IntentDialog, content: () -> Content) -> Self

static func result&lt;Value, Content>(value: Value, opensIntent: some AppIntent, dialog: IntentDialog, content: () -> Content) -> Self

Indicates the `AppIntent` finished performing

static func result&lt;Value, OpensAppIntent, Content>(value: Value, opensIntent: OpensAppIntent, dialog: IntentDialog, view: Content) -> Self

static func result&lt;Value, Content>(value: Value, opensIntent: some AppIntent, dialog: IntentDialog, view: Content) -> Self

Indicates the `AppIntent` finished performing

static func result&lt;Value, Content>(value: Value, opensIntent: some AppIntent, view: Content) -> Self

Indicates the `AppIntent` finished performing

static func result&lt;Value, OpensAppIntent, Content>(value: Value, opensIntent: OpensAppIntent, view: Content) -> Self

static func result&lt;Value, Content>(value: Value, view: Content) -> Self

Indicates the `AppIntent` finished performing

static func result&lt;Content>(view: Content) -> Self

Indicates the `AppIntent` finished performing

### Default Implementations

IntentResult Implementations

## Relationships

### Inherits From

- Sendable

### Inherited By

- OpensIntent
- ProvidesDialog
- ReturnsValue
- ShowsSnippetView

### Conforming Types

- IntentResultContainer

  Conforms when `Value` conforms to `_IntentValue`, `OpensAppIntent` conforms to `AppIntent`, `Snippet` is `_SnippetViewContainer`, `Dialog` conforms to `Copyable`, and `Dialog` conforms to `Escapable`.

## See Also

### Results

struct IntentResultContainer

An object that represents the output of a completed intent.

protocol OpensIntent

The result of performing an action that delivers an app intent back to the initiator of the action.

protocol ProvidesDialog

The result of performing an action that delivers a dialog back to the initiator of the action.

protocol ReturnsValue

The result of performing an action that delivers a value back to the initiator.

protocol ShowsSnippetView

The result of performing an action that delivers a view back to the initiator of the action.

protocol ResultsCollection

A protocol representing a collection of returned items with support for sectioning.

