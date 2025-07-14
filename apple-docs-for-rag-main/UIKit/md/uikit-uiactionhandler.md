

- UIKit
-  UIActionHandler 

Type Alias

# UIActionHandler

A type that defines the closure for an action handler.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
typealias UIActionHandler = (UIAction) -> Void
```

## Parameters 

`action`  

The action selected by the user.

## See Also

### Creating an action

convenience init(title: String, subtitle: String?, image: UIImage?, identifier: UIAction.Identifier?, discoverabilityTitle: String?, attributes: UIMenuElement.Attributes, state: UIMenuElement.State, handler: UIActionHandler)

Creates an action with the specified title, subtitle, image, identifier, discoverability title, attributes, state, and handler.

convenience init(title: String, image: UIImage?, identifier: UIAction.Identifier?, discoverabilityTitle: String?, attributes: UIMenuElement.Attributes, state: UIMenuElement.State, handler: UIActionHandler)

Creates an action with the specified title, image, identifier, discoverability title, attributes, state, and handler.

class func captureTextFromCamera(responder: any UIResponder &amp; UIKeyInput, identifier: UIAction.Identifier?) -> Self

Creates an action for capturing text using the device’s camera.

struct Identifier

A type that represents an action identifier.

