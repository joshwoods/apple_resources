

- App Intents
-  IntentResultContainer 

Structure

# IntentResultContainer

An object that represents the output of a completed intent.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct IntentResultContainer where Value : _IntentValue, OpensAppIntent : AppIntent
```

## Overview

Use the `IntentResult.result()` family of functions to create instances

## Topics

### Instance Properties

var activityIdentifier: String?

var dialog: IntentDialog?

var opensIntent: OpensAppIntent?

var value: Value?

### Default Implementations

IntentResult Implementations

## Relationships

### Conforms To

- Copyable
- IntentResult

  Conforms when `Value` conforms to `_IntentValue`, `OpensAppIntent` conforms to `AppIntent`, `Snippet` is `_SnippetViewContainer`, `Dialog` conforms to `Copyable`, and `Dialog` conforms to `Escapable`.

- OpensIntent

  Conforms when `Value` conforms to `_IntentValue`, `OpensAppIntent` conforms to `AppIntent`, `Snippet` conforms to `Copyable`, `Snippet` conforms to `Escapable`, `Dialog` conforms to `Copyable`, and `Dialog` conforms to `Escapable`.

- ProvidesDialog

  Conforms when `Value` conforms to `_IntentValue`, `OpensAppIntent` conforms to `AppIntent`, `Snippet` conforms to `Copyable`, `Snippet` conforms to `Escapable`, and `Dialog` is `IntentDialog`.

- ReturnsValue

  Conforms when `Value` conforms to `_IntentValue`, `OpensAppIntent` conforms to `AppIntent`, `Snippet` conforms to `Copyable`, `Snippet` conforms to `Escapable`, `Dialog` conforms to `Copyable`, and `Dialog` conforms to `Escapable`.

- Sendable
- ShowsSnippetView

  Conforms when `Value` conforms to `_IntentValue`, `OpensAppIntent` conforms to `AppIntent`, `Snippet` is `_SnippetViewContainer`, `Dialog` conforms to `Copyable`, and `Dialog` conforms to `Escapable`.

## See Also

### Results

protocol IntentResult

A type that contains the result of performing an action, and includes optional information to deliver back to the initiator.

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

