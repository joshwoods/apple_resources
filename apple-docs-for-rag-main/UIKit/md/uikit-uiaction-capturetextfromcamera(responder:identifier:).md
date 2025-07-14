

- UIKit
- UIAction
-  captureTextFromCamera(responder:identifier:) 

Type Method

# captureTextFromCamera(responder:identifier:)

Creates an action for capturing text using the device’s camera.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
@MainActor
class func captureTextFromCamera(
    responder: any UIResponder & UIKeyInput,
    identifier: UIAction.Identifier?
) -> Self
```

## Parameters 

`responder`  

The UIKeyInput responder to send the captureTextFromCamera(_:) message to.

`identifier`  

The unique identifier for the action. Specify `nil` to let this method create a unique identifier for you.

## See Also

### Creating an action

convenience init(title: String, subtitle: String?, image: UIImage?, identifier: UIAction.Identifier?, discoverabilityTitle: String?, attributes: UIMenuElement.Attributes, state: UIMenuElement.State, handler: UIActionHandler)

Creates an action with the specified title, subtitle, image, identifier, discoverability title, attributes, state, and handler.

convenience init(title: String, image: UIImage?, identifier: UIAction.Identifier?, discoverabilityTitle: String?, attributes: UIMenuElement.Attributes, state: UIMenuElement.State, handler: UIActionHandler)

Creates an action with the specified title, image, identifier, discoverability title, attributes, state, and handler.

struct Identifier

A type that represents an action identifier.

typealias UIActionHandler

A type that defines the closure for an action handler.

