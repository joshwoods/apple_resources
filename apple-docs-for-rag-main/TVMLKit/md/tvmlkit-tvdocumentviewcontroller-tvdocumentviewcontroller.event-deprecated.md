

- TVMLKit
- TVDocumentViewController
-  TVDocumentViewController.Event Deprecated

Structure

# TVDocumentViewController.Event

Events that can be triggered on the document view controller.

tvOS 13.0–18.0Deprecated

``` source
struct Event
```

Deprecated

Please use SwiftUI or UIKit

## Topics

### Initializers for Document View Controller Events

init(String)

Create a new document view controller event based on a string value.

init(rawValue: String)

Create an instance of a new document view controller event based on a string value.

### Event Types

static let appear: TVDocumentViewController.Event

An event that signals when the document appears.

static let disappear: TVDocumentViewController.Event

An event that signals when the document disappears.

static let highlight: TVDocumentViewController.Event

An event that signals when the document is highlighted.

static let holdSelect: TVDocumentViewController.Event

An event that signals when the document is held down and selected.

static let load: TVDocumentViewController.Event

An event that signals when the document is loaded.

static let play: TVDocumentViewController.Event

An event that signals when the document is played.

static let select: TVDocumentViewController.Event

An event that signals when the document is selected.

static let unload: TVDocumentViewController.Event

An event that signals when the document is unloaded.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

