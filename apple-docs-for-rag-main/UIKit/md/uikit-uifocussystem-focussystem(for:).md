

- UIKit
- UIFocusSystem
-  focusSystem(for:) 

Type Method

# focusSystem(for:)

Retrieves the focus system for the specified environment.

iOS 15.0+iPadOS 15.0+Mac CatalysttvOS 15.0+visionOS

``` source
@MainActor @preconcurrency
class func focusSystem(for environment: any UIFocusEnvironment) -> UIFocusSystem?
```

## Parameters 

`environment`  

The environment that the focus system contains.

## Discussion

This method returns `nil` if focus interaction isn’t supported or if the environment isn’t associated with a focus system.

## See Also

### Getting a focus system object

init?(for: any UIFocusEnvironment)

Retrieves a focus system object that contains the state information for the specified object.

Deprecated

