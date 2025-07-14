

- TVMLKit
-  TVDocumentViewController Deprecated

Class

# TVDocumentViewController

A view controller that represents a TVMLKit document.

tvOS 13.0–18.0Deprecated

``` source
@MainActor
class TVDocumentViewController
```

Deprecated

Please use SwiftUI or UIKit

## Overview

Instances of this class serve as bridges into `TVMLKit JS`’s document life cycle, and allow for native event handling with `TVMLKit`. This class also provides a way for native clients to communicate with `TVMLKit JS`.

## Topics

### Initializing the Document View Controller

convenience init(context: [String : Any], for: TVApplicationController)

Creates a new document view controller with a specific context and app controller.

### Managing Interactions with the Document

var delegate: (any TVDocumentViewControllerDelegate)?

The delegate for handling events in the document view controller.

protocol TVDocumentViewControllerDelegate

Methods to manage updates, events, and errors from the document view controller.

### Handling Document Events

struct Event

Events that can be triggered on the document view controller.

### Updating the Document View Controller

func update(using: [String : Any])

Updates the document view controller with the provided context.

### Accessing the Document’s Components

var appController: TVApplicationController?

The document’s app controller that bridges UI, navigation stack, storage, and event handling from JavaScript.

var documentContext: [String : Any]

The current document context.

## Relationships

### Inherits From

- UIViewController

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSExtensionRequestHandling
- NSObjectProtocol
- Sendable
- UIAppearanceContainer
- UIContentContainer
- UIFocusEnvironment
- UIResponderStandardEditActions
- UIStateRestoring
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### Views and View Controllers

class TVViewElement

A representation of a read-only DOM node.

Deprecated

protocol TVInterfaceCreating

A protocol that defines methods used to create views and view controllers.

Deprecated

class TVInterfaceFactory

A factory for the creation of views and view controllers.

Deprecated

class TVBrowserViewController

A view controller that presents content in a browsable, full-screen format.

