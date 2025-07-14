

- TVMLKit
-  TVViewElement Deprecated

Class

# TVViewElement

A representation of a read-only DOM node.

tvOS 9.0–18.0Deprecated

``` source
class TVViewElement
```

Deprecated

Please use SwiftUI or UIKit

## Overview

The `TVViewElement` model object is traversed by the TVInterfaceFactory factory to construct views and view controllers, and to render templates. Views and view controllers should use the available dispatch APIs to send user events to JavaScript.

## Topics

### Inspecting a View Element

var autoHighlightIdentifier: String?

A string identifying the element that is initially in focus.

var attributes: [String : String]?

The attributes associated with a view element.

var children: [TVViewElement]?

An array containing the child elements of the element currently being inspected.

var isDisabled: Bool

Boolean value indicating whether the current element being inspected is disabled.

var identifier: String

A string containing the unique identifier for an element.

var name: String

A string containing the element’s name.

var parent: TVViewElement?

The parent of the current node.

var style: TVViewElementStyle?

The style applied to an element.

var updateType: TVElementUpdateType

The value that describes any changes to the DOM tree after it has been reparsed.

enum TVElementUpdateType

Describes any changes to the DOM tree after it has been reparsed.

### Dispatching Events

func dispatchEvent(type: TVElementEventType, canBubble: Bool, cancellable: Bool, extraInfo: [String : Any]?, completion: ((Bool, Bool) -> Void)?)

Dispatches an event of a specific type to the JavaScript file.

enum TVElementEventType

The type of event that has been dispatched.

func dispatchEvent(name: String, canBubble: Bool, cancellable: Bool, extraInfo: [String : Any]?, completion: ((Bool, Bool) -> Void)?)

Dispatches a custom-named event.

### Resetting a Property’s Value

func resetProperty(TVElementResettableProperty)

Resets the property to its default value.

enum TVElementResettableProperty

The types of properties that can be reset to their default values.

### Instance Properties

var elementData: [String : Any]

## Relationships

### Inherits From

- NSObject

### Inherited By

- TVImageElement
- TVTextElement

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Views and View Controllers

protocol TVInterfaceCreating

A protocol that defines methods used to create views and view controllers.

Deprecated

class TVInterfaceFactory

A factory for the creation of views and view controllers.

Deprecated

class TVBrowserViewController

A view controller that presents content in a browsable, full-screen format.

class TVDocumentViewController

A view controller that represents a TVMLKit document.

Deprecated

