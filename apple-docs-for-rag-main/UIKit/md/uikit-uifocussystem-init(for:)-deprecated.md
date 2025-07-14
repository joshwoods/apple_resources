

- UIKit
- UIFocusSystem
-  init(for:) Deprecated

Initializer

# init(for:)

Retrieves a focus system object that contains the state information for the specified object.

iOS 12.0–15.0DeprecatediPadOS 12.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedtvOS 12.0–15.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
init?(for environment: any UIFocusEnvironment)
```

## Parameters 

`environment`  

The object whose state you want to return. Specify the view, view controller, or window whose state you want. You can also specify any other object that adopts the UIFocusEnvironment protocol.

## Return Value

The UIFocusSystem object that manages the state for the specified object or `nil` if focus interactions are not available for the object.

## See Also

### Getting a focus system object

class func focusSystem(for: any UIFocusEnvironment) -> UIFocusSystem?

Retrieves the focus system for the specified environment.

