

- App Intents
-  ProvidesDialog 

Protocol

# ProvidesDialog

The result of performing an action that delivers a dialog back to the initiator of the action.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol ProvidesDialog : IntentResult where Self.Dialog == IntentDialog
```

## Relationships

### Inherits From

- IntentResult
- Sendable

### Conforming Types

- IntentResultContainer

  Conforms when `Value` conforms to `_IntentValue`, `OpensAppIntent` conforms to `AppIntent`, `Snippet` conforms to `Copyable`, `Snippet` conforms to `Escapable`, and `Dialog` is `IntentDialog`.

## See Also

### Results

protocol IntentResult

A type that contains the result of performing an action, and includes optional information to deliver back to the initiator.

struct IntentResultContainer

An object that represents the output of a completed intent.

protocol OpensIntent

The result of performing an action that delivers an app intent back to the initiator of the action.

protocol ReturnsValue

The result of performing an action that delivers a value back to the initiator.

protocol ShowsSnippetView

The result of performing an action that delivers a view back to the initiator of the action.

protocol ResultsCollection

A protocol representing a collection of returned items with support for sectioning.

