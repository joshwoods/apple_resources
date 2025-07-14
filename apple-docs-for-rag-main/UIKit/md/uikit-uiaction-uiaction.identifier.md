

- UIKit
- UIAction
-  UIAction.Identifier 

Structure

# UIAction.Identifier

A type that represents an action identifier.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
struct Identifier
```

## Topics

### Constants

static let paste: UIAction.Identifier

Identifies the action that pastes the current contents of the pasteboard into your app’s interface.

static let pasteAndGo: UIAction.Identifier

Identifies the action that pastes the current contents of the pasteboard into your app’s interface and navigates to the entity it references.

static let pasteAndMatchStyle: UIAction.Identifier

Identifies the action that pastes the current contents of the pasteboard into your app’s interface using the text style of the target.

static let pasteAndSearch: UIAction.Identifier

Identifies the action that pastes the current contents of the pasteboard into your app’s interface and performs a search.

### Initializers

init(String)

Creates an action identifier from the specified string.

init(rawValue: String)

Creates an action identifier from the specified string.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Creating an action

convenience init(title: String, subtitle: String?, image: UIImage?, identifier: UIAction.Identifier?, discoverabilityTitle: String?, attributes: UIMenuElement.Attributes, state: UIMenuElement.State, handler: UIActionHandler)

Creates an action with the specified title, subtitle, image, identifier, discoverability title, attributes, state, and handler.

convenience init(title: String, image: UIImage?, identifier: UIAction.Identifier?, discoverabilityTitle: String?, attributes: UIMenuElement.Attributes, state: UIMenuElement.State, handler: UIActionHandler)

Creates an action with the specified title, image, identifier, discoverability title, attributes, state, and handler.

class func captureTextFromCamera(responder: any UIResponder &amp; UIKeyInput, identifier: UIAction.Identifier?) -> Self

Creates an action for capturing text using the device’s camera.

typealias UIActionHandler

A type that defines the closure for an action handler.

