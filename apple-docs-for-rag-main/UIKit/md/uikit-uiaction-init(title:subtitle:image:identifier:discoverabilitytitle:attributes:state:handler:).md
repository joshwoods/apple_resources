

- UIKit
- UIAction
-  init(title:subtitle:image:identifier:discoverabilityTitle:attributes:state:handler:) 

Initializer

# init(title:subtitle:image:identifier:discoverabilityTitle:attributes:state:handler:)

Creates an action with the specified title, subtitle, image, identifier, discoverability title, attributes, state, and handler.

iOS 15.0+iPadOS 15.0+Mac CatalysttvOS 15.0+visionOS

``` source
@MainActor @preconcurrency
convenience init(
    title: String = "",
    subtitle: String? = nil,
    image: UIImage? = nil,
    identifier: UIAction.Identifier? = nil,
    discoverabilityTitle: String? = nil,
    attributes: UIMenuElement.Attributes = [],
    state: UIMenuElement.State = .off,
    handler: @escaping UIActionHandler
)
```

## Parameters 

`title`  

The title to display for the action.

`subtitle`  

The subtitle to display alongside the action’s title.

`image`  

The image to display next to the action’s `title`. Only the context menu system supports the display of an image, and only when the app is running in iOS.

`identifier`  

The unique identifier for the action. Specify `nil` to let this method create a unique identifier for you.

`discoverabilityTitle`  

An elaborated title that explains the purpose of the action.

`attributes`  

The attributes indicating the style of the action.

`state`  

The initial state of the action.

`handler`  

The handler to invoke after a person selects the action. This handler has the following parameter:

action  
The action that a person selects.

## See Also

### Creating an action

convenience init(title: String, image: UIImage?, identifier: UIAction.Identifier?, discoverabilityTitle: String?, attributes: UIMenuElement.Attributes, state: UIMenuElement.State, handler: UIActionHandler)

Creates an action with the specified title, image, identifier, discoverability title, attributes, state, and handler.

class func captureTextFromCamera(responder: any UIResponder &amp; UIKeyInput, identifier: UIAction.Identifier?) -> Self

Creates an action for capturing text using the device’s camera.

struct Identifier

A type that represents an action identifier.

typealias UIActionHandler

A type that defines the closure for an action handler.

